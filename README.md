# COVID-19 Projection in the US

Projections of COVID-19 in the US at county level generated based on latest data.

Generated by Shaman group.

Projection visualizations, descriptions, and associated publications can be found here: https://blogs.cuit.columbia.edu/jls106/publications/covid-19-findings-simulations/

County-level case and death data are compiled from USAFACTS. https://usafacts.org/visualizations/coronavirus-covid-19-spread-map/

Projections are generated for daily new confirmed case, daily new infection (both reported and unreported), cumulative demand of hospital beds, ICU and ventilators as well as daily mortality (2.5, 25, 50, 75 and 97.5 percentiles). 

Projections make assumptions about how the transmission parameters 

Scenarios

May 3 - Present: Reopening
We modified our control scenarios to account for increases in contact rates due to
loosening restrictions in states that have begun to reopen economically. We project
four scenarios. In states maintaining or increasing current
social distancing restrictions, we continue to apply the 20% weekly reductions of contact
rates, as in the 20% contact reduction Adaptive intervention scenario described below. However, in states that reopen, we apply an increase to the contact rate of counties in those states. In the first scenario, we apply a one-time 10%
increase to the contact rate during the week that the state is scheduled to reopen and
maintain this new increased rate for the remainder of the projection. In the second
scenario, the contact rate is increased by an additional 10% each week to represent
progressive loosening of restrictions and increased public confidence and frequenting of
businesses.  The third and fourth scenarios are the same as the first and second scenarios, but with a 5% rather than 10% increase in contact rate in reopening states.

April 5 - April 26: Adaptive interventions
Four different adaptive scenarios of contact reduction were projected, 0% (no contact reduction via social distancing controls and behavior change), 20%, 30%, and 40% contact reduction. These scenarios are meant to mimic adaptive adjustments in contact imposed both by government regulations (e.g. school closures, restrictions on mass gatherings) and population self-regulation (e.g. isolation, mask wearing, social distancing).  Upon initiation of projections on a given day, all counties with 10 or more confirmed cases impose a 0%, 20%, 30% or 40% contact rate reduction, depending on the projection scenario; all other counties implement no contact reduction.  Each week following, if a county newly exceeds 10 confirmed cases, a 0%, 20%, 30% or 40% contact rate reduction is imposed, depending on the projection scenario. Counties that had previously exceeded 10 confirmed cases and also experience an increase in the number of weekly reported confirmed cases impose a further, multiplicative 0%, 20%, 30% or 40% contact rate reduction, depending on the projection scenario.  Counties with fewer than 10 confirmed cases continue not to implement control.  This multiplicative ratcheting of contact reduction levels is continued until the end of simulations and is meant to represent increasing reactive social distancing imposed within counties as long as confirmed weekly cases of COVID-19 continue to rise.
 
Note that in these scenarios, contact reductions are never relaxed.  Once weekly new confirmed cases decrease, the county simply stays at its current level of control.

Projections for daily new confirmed case and daily new infection are reported in Projection_nointerv.csv, Projection_80contact.csv,  Projection_70contact.csv and Projection_60contact.csv

Projections for cumulative demand of hospital beds, ICU, ventilators and daily mortality are reported in bed_nointerv.csv, bed_80contact.csv, bed_70contact and bed_60contact.csv.

Note that hospitalizations and ICU bed numbers indicate the current demand on a given day (NOT just the new persons needing beds).

Note, the NY metropolitan area in the figure includes 11 counties: Kings County NY, Queens County NY, New York County NY, Bronx County NY,Richmond County NY, Westchester County NY, Bergen County NJ, Hudson County NJ, Passaic County, NJ, Putnam County NY, Rockland County NY

Interpretation Considerations

Several qualifications with respect to these projections must be noted and considered during interpretation.  Firstly, the model is optimized using observations through the projection date; however, those observations, i.e. confirmed cases by county, represent infections that were acquired by individuals 1-2 weeks earlier during a time prior to the implementation of many of the social distancing and isolation measures in place on the projection date. Because of this long delay between infection acquisition and case confirmation, any flattening of the curve due to these effects is not yet apparent in observations nor communicated to the model during optimization. Consequently, the no intervention scenario roughly represents the transmission potential of the virus around March 12th projected forward.  As many new control policies were effected after March 12, 2020, the contact reduction projections may depict paths that some counties are already following and thus may be more representative of future activity.  In this fashion, the 3 scenarios provide references against which the effectiveness of control measures already enacted can be assessed.  We also ask readers to note the cones of uncertainty associated with each scenario projection, which broaden into the future.

Secondly, the landscape to which this model has been optimized is highly variable in space and time, due to differences in contact behavior, population density, control measures and testing practices. These differences in space and time make the fitting of any model of this scale challenging. In this shifting landscape, it is very important to reiterate that it will take 10-14 days before the effects of real-world interventions—any flattening of the curve weeks—become apparent.

# Citation

Please cite: Sen Pei, Jeffrey Shaman, Initial Simulation of SARS-CoV2 Spread and Intervention Effects in the Continental US. medRxiv.doi: https://doi.org/10.1101/2020.03.21.20040303

