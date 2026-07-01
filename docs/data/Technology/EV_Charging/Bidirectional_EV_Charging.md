> [!NOTE] 
> This is a source file for the [Electricity Sector Field Guide](https://grahamlea.github.io/Electricity-Sector-Field-Guide/)
> It uses a very small subset of Markdown in a specific format.
> See `data/README.md` for details.

# Bidirectional EV Charging
#UsedVeryFrequently

## Synonyms
- Vehicle to Grid (V2G)
- Vehicle to Home (V2H)
- Vehicle to Load (V2L)
- Vehicle to Vehicle (V2V)

## Abbreviations
- V2X
- Bidi


## Summary

Dispatching [power] from an [electric vehicle]'s main [battery] to supply circuits or appliances
external to the vehicle.


## More

The intended destination of the power determines more specific sub-types:
"Vehicle to Home" (V2H) when the EV is supporting power usage in a property
via the property's circuits (typically with load-following);
"Vehicle to Grid" (V2G) when power is being sent into a wider [grid];
"Vehicle to Load" (V2L) when supporting a small number of appliances directly;
"Vehicle to Vehicle" (V2V) when using one EV to directly charge another EV.
V2X means "Vehicle to Everything", encompassing all of the above,
and synonymous with bidirectional charging.

The first generation of EVs and chargers ([EVSE]) were all "unidirectional", 
meaning power only ever flows into the vehicle.
Unidirectional equipment and protocols are sometimes referred to as "V1G".

V2G, V2H, and V2L all supply [alternating current] (AC), 
which means an [inverter] is needed to convert from the battery's [direct current] (DC).
V2L is provided using an inverter onboard the vehicle, 
and delivered via either a standard AC socket in the vehicle, 
or an adapter that plugs into the charging port and provides an AC socket.
V2G and V2H may use an inverter onboard the vehicle, delivering AC power to the EVSE via the charging port. 
Alternatively, the EVSE may pull DC power out of the vehicle and convert it using its own inverter.
The industry appears to be leaning towards preferring the DC option 
with external inverters deployed in EVSE (as of 2026).

V2V charging can be implemented using AC or DC power.
It is not widely supported by vehicles at present (2026).

The [ISO 15118]-20 standard for vehicle to charger communication,
and the [OCPP] 2.1 protocol for charger to [CSMS] communication,
include protocols for standardised implementation of V2H and V2G.
V2G has been demonstrated using proprietary methods, and custom extensions to earlier protocols.
The CHAdeMO charging standard has included V2G since 2014.

Note that some sources define V2H as only covering when
a property being supplied power is [islanded] from the grid.
Others distinguish explicitly between grid-connected V2H and islanded V2H.
Some sources use V2X/G/H/V to describe information flows and communication technology,
rather than energy flows.


## Links
- [What is bidirectional charging? @ SolarQuotes](https://www.solarquotes.com.au/electric-vehicles/v2l-v2g-v2h/)
- [Vehicle-to-grid @ Wikipedia](https://en.wikipedia.org/wiki/Vehicle-to-grid) 
- [V2G, V2H, and V2L Explained @ Ocular Charging](https://www.youtube.com/watch?v=lqhwSVjlCxQ) #video
