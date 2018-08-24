+++
# Date this page was created.
date = "2009-09-20"

# Project title.
title = "Fuel Cell Durability (PhD Project)"
slug = "fuelcelldura"
# Project summary to display on homepage.
summary = "A hydrogen fuel cell does not last because platinum is electrochemically unstable. A cathode catalyst can be made more stable if it posses some oxygen evolution activity in addition to oxygen reduction activity. Will the addition of iridium and ruthenium to platinum help to create a more stable catalyst?" 

# Optional image to display on homepage (relative to `static/img/` folder).
image_preview = "disksputholder.jpg"

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
#tags = ["deep-learning"]
tags = []
# Optional external URL for project (replaces project detail page).
external_link = ""

# Does the project detail page use math formatting?
math = false

# Optional featured image (relative to `static/img/` folder).
[header]
image = "disksputholder.jpg"
#image = "rcdm_scheme.jpg"
caption = "Catalyst coated disk samples fresh out of the sputtering chamber :smile:"

+++
## Summary
When a hydrogen fuel cell is started, hydrogen gas will occupy only a portion of the anode flow field. Something similar happens during shut down due to air diffusing back into the anode; a region will be rich in fuel and the remainder of the flow field will be fuel starved. In either case, the presence of a hydrogen-air front creates an internal voltage in the fuel cell severe enough to corrode both the platinum and the carbon components comprising the current collector. Iridium and Ruthenium can preserve the carbon and platinum by catalyzing the oxygen evolution reaction in favour of the carbon corrosion reaction. Shown below are the electrochemical reactions in the fuel rich and fuel starved regions, along with their electronic and ionic pathways. 
![The Reverse Current Decay Mechanism](/img/rcdm_blog.png "How a fuel cell catalyst degrades")
Ruthenium is cheaper, more active, but less stable than Iridium, so the mixture should be carefully optimized. Rotating disk electrodes are preferred to fuel cells for studying catalyst stability. Start up and shut down events are simulated with a repeating sequence of galvanostatic and potentiostatatic holds. The finished thesis document can be found [here](http://dalspace.library.dal.ca/handle/10222/73297).