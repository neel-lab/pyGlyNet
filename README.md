# pyGlyNet
## Classes
### Monosaccharide
*.isMono*: Boolean, if it is a monosaccharide<br/>
*.mlong*: String with Hex, HexNAc representation<br/>
*.symbol*: Single letter for each monosaccharide [n,h,s etc.]<br/>
*.mmass*: monoisotopic mass<br/>
### Glycan
*.conc*: Concentration and units<br/>
*.loc*: Compartment location of glycan<br/>
*.gtype*: Returns HexHexNAc and also symbolic form <br/>
*.isglycan*: Boolean return if it a glycan<br/>
*.gmass*: Glycan mass<br/>
*.getbranch*: Determines the location of branch in IUPAC condensed string<br/>
*.antennae*: Find the antennae within glycan<br/>
*.sameglycan*: Compare two glycans<br/>
*.alternateForms*: Alternate expressions for IUPAC string<br/>
*.antennaeMinusOne*: List of glycans formed upon removing one antennae<br/>
*.checkmotif*: Determines if motif appears in the glycan and if so how many times and where<br/>
*.distanceMartix*: not yet ready<br/>
### Enzyme
*.isOgly*: Boolean of enzyme is O-glycosylation specific<br/>
*.bi*: Boolean if this is a bimolecular reaction rule<br/>
*.domain*:Boolean of enzyme designed for specific domain, e.g EGF <br/>
*.enzType* Enzyme properties getString, putString and constraint<br/>
### speciesList
*This is a list of dictionaries with each dictionary corresponding to a glycan*<br/>
*.addSpecies*: Add species to speciesList<br/>
*.removeSpecies*: Remove species to speciesList<br/>
*.removeDuplicate*: Remove duplicate species, if present<br/>
### enzymeList
*This is a list of dictionaries with each dictionary corresponding to a enzyme*<br/>
*.addEnzyme*: Add an enzyme to list<br/>
*.removeEnzyme*: Remove enzyme from list<br/>
*.removeDuplicate*: Remove duplicate enzyme from list<br/>
### reaction
*.constraint*: To check if constraint condition satisfied<br/>
*.inferProduct*: For building forward reaction<br/>
*.inferReactant*: For reverse reaction synthesis<br/>
### Network
*.addReaction*: Add reaction to network<br/>
*.removeReaction*: Remove reaction from network<br/>
*.removeDuplicate*: Remove duplicate reactions in the network<br/>
*.buildForward*: Synthesize a forward reaction network<br/>
*.buildReverse*: Build a reaction network given some of the products detected<br/>
### Compartment
Define compartment *name*, *size* and *residence time*<br/>
### OtherDef 
*Contains class independent functions for string manipulation and program validation*<br/>
*strpos*: To find all positions of match inside string<br/>
*reString_glycan*: Only works on … and <> features<br/>
*reString*: sort of restring variant<br/>
*string2List*: Convert gString and pString into list when there are \| objects in reaction rule<br/>
*genEnzRules*: Reads excel file and extracts enzyme rules from it. Needed to build enzyme class<br/>
*join*: used to concatenate strings<br/>
*checkRxnRules*: Makes sure that the excel sheet containing reaction rules is well parsed<br/>
