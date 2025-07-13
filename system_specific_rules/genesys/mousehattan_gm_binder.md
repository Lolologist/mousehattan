<style>
 .phb code {
     font-size:10px;
     padding-top: 0px;
     padding-bottom: 0px;
 }
/* IMPORTS */

@import url('https://fonts.googleapis.com/css?family=Crimson+Text:400,600,600i,700');

/* Main Background */
  .phb { background-image: url("https://www.gmbinder.com/images/5s6VJkT.png"); text-align:justify; text-indent:0px;}

/* Fonts */

.phb {
    font-family: 'Crimson Text', serif;
}

.phb h1, .phb h2, .phb h3, .phb h4, .phb h5, .phb h6 { 
    letter-spacing: 0.6px;
    font-family: 'Bebas Neue';
}

.phb h1{
    color: #1ABEEF;
    font-weight:400;
    font-variant: uppercase;
    font-size:42pt;
    margin-bottom:30px;
}

/* Makes the bigger "first letter" in paragraphs under H1 and H2*/
.phb h1 + p:first-letter, .phb h2 + p:first-letter  {
    font-family: 'Crimson Text';
    color: #326DA1;
    font-size:32pt;    
    line-height:95%;
    margin-bottom:-9px;
    margin-right:2px;
    margin-top:-5px;
    float:left;
}

.phb h2 {
    color: #1ABEEF;
    font-variant: small-caps;
    display:table;
    font-size:32pt;
    font-weight:300;
    column-span:all;
}

/* create the offset underline under h2s */
.phb h2:after {
    content:"";
    border-bottom: 2px solid #CCCCCC;
    display: table;
    width:100%;
    margin-top:-5px;
    margin-left:20px;
}

.phb h3 {
    color: #1ABEEF;
    font-variant: small-caps;
    font-size: 18pt;
    font-weight:1;
    border:none;
}

.phb h4 {
    color: #ed9629;
    font-variant: small-caps;
    font-size: 16pt;
    text-align:center;
}

.phb h5 {
    color: #326DA1;
    font-weight: 1;
    font-variant: small-caps;
    font-size: 16pt;
}

.phb h6 {
    color: #ea702b;
    font-variant: small-caps;
    font-size: 16pt;
    display: table;
    border-bottom: 1px solid #ea702b;
}

.phb p { 
    font-size: 15px; 
  	letter-spacing: -0.4px;
  	line-height:1.15em;
  	text-indent:0px !important;
  	font-weight:400;
  	padding-bottom:1px;
  	column-fill:balance;
  }
  
.phb p + p {
    margin-top:0px;  
  }

.phb wide {clear:both;}
.phb ul {list-style: none;}
.phb ul li::before {
    content: """; 
    color: #F69337;
    display: inline-block;
    width: 1em;
    margin-left: -1em;
  }

/* Tables */
.phb td {
    font-family: 'Crimson Text', serif;
    font-size:8pt;
    font-weight:400;
    text-align:left;
}
.phb td, th {border: 1px solid gray;}
.phb table {overflow:auto;}
.phb table tr:nth-child(odd) td {background-color: #E0F4FC;}
.phb table thead th {
    color: white; 
    background-color: #F69337; 
  	padding-top: 0.3em;
    padding-left: 0.5em;
    text-transform: uppercase;
}
.phb table tbody tr td {  padding: 0.5em;}
.phb table thead {display: table-row-group; }
.phb table .subheader td {
    color:white;
    text-transform:uppercase;
    padding-bottom:2px;
    background-color: #2D4864 !important;
    font-size:10pt;
    font-weight:bold;
    }

/* Genesys Notes */

.phb .note
{
    position:relative;
    color: white;
    background-color: #2D4864;
    border-radius: 0px 0px 30px 0px;
    padding: 10px 20px;  
    font-family: 'Crimson Text';
    letter-spacing: 0.5px;
    font-size:12ptx;
    font-weight:600
    }    

.phb .note:before {
    position:absolute;
    content:" ";
    border-style:solid;
    border-width:1px;
    -moz-border-image: -moz-linear-gradient(-45deg, rgba(219,219,219,.7) 0%, rgba(219,219,219,0) 50%, rgba(219,219,219,0) 100%);
    -webkit-border-image: -webkit-linear-gradient(-45deg, rgba(219,219,219,.7) 0%,rgba(219,219,219,0) 50%,rgba(219,219,219,0) 100%);
    border-image: linear-gradient(135deg, rgba(219,219,219,.7) 0%,rgba(219,219,219,0) 50%,rgba(219,219,219,0) 100%); 
    left:4px;
    top:4px;
    right:4px;
    bottom:4px;
    border-image-slice:1;
}

.phb .note h5 {color:white;}
.phb .note td {color:black;}
.phb .note table tr:nth-child(even) td { background-color: #ffffff;}
  
  
/* Example Block */

.phb .example
{
    position:relative;
    color: black;
    background: rgba(204, 203, 199, 0.4);
    border-radius: 0px 0px 30px 0px;
    padding: 14px 20px;
}

/* Read-aloud */

.phb .read {
    display:block;
    font-family: 'Crimson Text';
    font-size:10pt;
    font-style: italic;
    color: rgb(230,0,0);
    border: 1px dotted rgb(230,0,0);
    border-radius:30px;
    padding:15px;
    position:relative;
}

.phb .read:before {
    content:'';
    position:absolute;
    display:block;
    border: 1px dotted rgb(230,0,0);
    border-radius:30px;
    left:2px;
    top:2px;
    right:2px;
    bottom:2px;
    }

/* Footer */
.phb .pageNumber { color: #000000}
.phb .footnote { color: #000000 }
.phb:nth-child(odd) .pageNumber { color: black;
	right: 40px;
	bottom: 52px;
	width: 50px;
	text-align: center;
    font-family: 'Bebas Neue';
    font-size:11pt;
    font-weight:bold;
}

.phb:nth-child(even) .pageNumber { color: black;
	left: 40px;
	bottom: 52px;
	width: 50px;
    text-align: center;
    font-family: 'Bebas Neue';
    font-size:11pt;
    font-weight:bold;
}

.phb .footnote { color: black 
    font-family: 'Bebas Neue' 
    font-weight: bold 
    vertical-align: center;
    padding-top:11px;
}

.phb:nth-child(even) .footnote {border-left:2px solid black;
    padding-left:6px;
}

.phb:nth-child(odd) .footnote {border-right:2px solid black;
    padding-right:6px;
}

.phb:after { 
    background-image:url("none") 
}



/* Dice and Symbols */

@font-face {
  font-family: 'Genesys';
  src: local('Genesys');
}
.phb .symbols {
    font-family: Genesys;
}

@font-face {
  font-family: 'Genesys1';
  src: local('EotE Symbol');
}
.phb .dice {
    font-family: Genesys1;
}


.phb .setback {
    font-family: Genesys1;
    color: black;
    text-shadow: -1px 0 #000000,0 1px #000000,1px 0 #000000,0 -1px #000000;
}

.phb .note .setback, .phb .note .boost, .phb .note .challenge, .phb .note .proficiency, .phb .note .difficulty, .phb .note .ability {
    text-shadow: -1px 0 #ffffff,0 1px #ffffff,1px 0 #ffffff,0 -1px #ffffff;
}

.phb .note  td > .setback, .phb .note td > .boost, .phb .note td > .challenge, .phb .note td > .proficiency, .phb .note td >  .difficulty, .phb .note td.ability {
    text-shadow:  -1px 0 #000000,0 1px #000000,1px 0 #000000,0 -1px #000000;
}

.phb .boost {
    font-family: Genesys1;
    color: #76CDDB;
    text-shadow: -1px 0 #000000,0 1px #000000,1px 0 #000000,0 -1px #000000;
}

.phb .challenge {
    font-family: Genesys1;
    color: #751317;
    text-shadow: -1px 0 #000000,0 1px #000000,1px 0 #000000,0 -1px #000000;
}

.phb .proficiency {
    font-family: Genesys1;
    color: #FEF035;
    text-shadow: -1px 0 #000000,0 1px #000000,1px 0 #000000,0 -1px #000000;
}

.phb .difficulty {
    font-family: Genesys1;
    color: #52287E;
    text-shadow: -1px 0 #000000,0 1px #000000,1px 0 #000000,0 -1px #000000;
}

.phb .ability {
    font-family: Genesys1;
    color: #46AC4E;
    text-shadow: -1px 0 #000000,0 1px #000000,1px 0 #000000,0 -1px #000000;
}


/* Archetypes */

.phb .archetype {
    background-image: url('https://www.gmbinder.com/images/wk1XTwj.png');
    height:62px;
    width:329px;
    background-size:100%;
    font-family: 'Bebas Neue';
    font-size:14pt;

    }

.phb .archetype .bra {
    position:relative;
    left:14px;
    top:6px;
    text-align:center;
    display:inline-block;
    width:25px;
}

.phb .archetype .agi {
    position:relative;
    left:42px;
    top:6px;
    width:25px;
    text-align:center;
    display:inline-block;
}
.phb .archetype .int {
    position:relative;
    left:68px;
    top:6px;
    width:25px;
    text-align:center;
    display:inline-block;
}

.phb .archetype .cun {
    position:relative;
    left:95px;
    top:6px;
    width:25px;
    text-align:center;
    display:inline-block;
}
.phb .archetype .wil {
    position:relative;
    left:122px;
    top:6px;
    width:25px;
    text-align:center;
    display:inline-block;
}
.phb .archetype .pre {
    position:relative;
    left:148px;
    top:6px;
    width:25px;
    text-align:center;
    display:inline-block;
}
/* Adversaries */

.phb .adversary {
    background-image: url('https://www.gmbinder.com/images/ks1JaPU.png');
    height:47px;
    width:329px;
    background-position: -3px 0px;
    background-size:102%;
    font-family: 'Bebas Neue';
    font-size:14pt;
}

.phb .adversary .soak {
    position:relative;
    left:26px;
    top:13px;
    width:25px;
    text-align:center;
    display:inline-block;
}
.phb .adversary .wound {
    position:relative;
    left:79px;
    top:13px;
    width:25px;
    text-align:center;
    display:inline-block;
}
.phb .adversary .strain {
    position:relative;
    left:135px;
    top:13px;
    width:25px;
    text-align:center;
    display:inline-block;
}
.phb .adversary .mdef {
    position:relative;
    left:176px;
    top:13px;
    width:25px;
    text-align:center;
    display:inline-block;
}
.phb .adversary .rdef {
    position:relative;
    left:175px;
    top:13px;
    width:25px;
    text-align:center;
    display:inline-block;
}

/* MINION STAT BLOCK */

.phb .minion {
    background-image: url('https://www.gmbinder.com/images/K1aEwZa.png');
    height:63px;
    width:329px;
    background-position: 42px 0px;
    background-repeat:no-repeat;
    background-size:75%;
    font-family: 'Bebas Neue';
    font-size:14pt;
}

.phb .minion .soak {
    position:relative;
    left:71px;
    top:13px;
    width:25px;
    text-align:center;
    display:inline-block;
}

.phb .minion .wound {
    position:relative;
    left:125px;
    top:13px;
    width:25px;
    text-align:center;
    display:inline-block;
}

.phb .minion .mdef {
    position:relative;
    left:165px;
    top:13px;
    width:25px;
    text-align:center;
    display:inline-block;
}
.phb .minion .rdef {
    position:relative;
    left:165px;
    top:13px;
    width:25px;
    text-align:center;
    display:inline-block;
}

/* Vehicles */

.phb .vehicle {
    background-image: url('https://www.gmbinder.com/images/JEgri2b.png');
    height:80px;
    width:329px;
    background-size: 100%;
    background-repeat:no-repeat;
    font-family: 'Bebas Neue';
    font-size:14pt;
}


.phb .vehicle .sil {
    position:relative;
    left:14px;
    top:6px;
    text-align:center;
    display:inline-block;
    width:25px;
}

.phb .vehicle .speed {
    position:relative;
    left:41px;
    top:6px;
    text-align:center;
    display:inline-block;
    width:25px;
}

.phb .vehicle .hand {
    position:relative;
    left:67px;
    top:6px;
    text-align:center;
    display:inline-block;
    width:25px;
}

.phb .vehicle .armor {
    position:relative;
    left:107px;
    top:12px;
    text-align:center;
    display:inline-block;
    width:25px;
}
.phb .vehicle .def {
    position:relative;
    left:163px;
    top:12px;
    text-align:center;
    display:inline-block;
    width:25px;    
}
.phb .vehicle .ht {
    position:relative;
    left:53px;
    top:53px;
    text-align:center;
    display:inline-block;
    width:25px;    
}

.phb .vehicle .ss {
    position:relative;
    left:107px;
    top:53px;
    text-align:center;
    display:inline-block;
    width:25px;    
}

/*Index*/

.phb .index-letter {
    color:rgb(118,18,19);
    font-size:24pt;font-weight:bold; 
    font-family:'Bebas Neue';
    line-height:1.1em;
}

.phb .index {
    list-style:none;
    padding:0;
    overflow-x:hidden;
    max-width:329px;
}

.phb .index li::before {
            content: ""; }
            
.phb .index li {
    
    display:flex;
}
            
.phb .index li span:first-child {
    margin-right:0.2em;
    order:1;
}
            
.phb .index li::after {
  content: "";
  border-bottom: 1px dotted;
  flex-grow: 1;
  order: 2;
  position:relative;
  top:-5px
}

.phb .index span + span {
    order:3;
    margin-left:0.2em;
    }
    
/* NON BLENDED IMAGE BORDER */
    
.phb .non-blended {
    padding:10px;
    border-width:2px;
    border-style:solid;
    border-image:linear-gradient(135deg, rgba(230,0,0,1) 0%,rgba(230,0,0,0.01) 99%,rgba(230,0,0,0) 100%);
    -moz-border-image:-moz-linear-gradient(-45deg, rgba(230,0,0,1) 0%, rgba(230,0,0,0.01) 99%, rgba(230,0,0,0) 100%); -webkit-border-image:-webkit-linear-gradient(-45deg, rgba(230,0,0,1) 0%,rgba(230,0,0,0.01) 99%,rgba(230,0,0,0) 100%);
    border-image-slice: 1;
}


</style>


# The Great Burrow
*A Complete Campaign Guide for Genesys RPG*

Welcome to the forest metropolis where tiny paws built impossible dreams. The Great Burrow is a sprawling city of woodland creatures that rivals any great metropolis in scope, ambition, and complexity. From the vertical maze of Mousehattan's carved stone chambers to the canopy highways of The Branchx, from the buzzing agricultural powerhouse of The Hives to the working waterfront of Lin's Brook, and finally to the forgotten island where Rangers stand between civilization and chaos.

This is a city where squirrels build rope bridges between skyscrapers of bark and leaf, where beaver-engineered dams power workshops that never sleep, where organized crime families of rats control the shadows while mice cling to old money and older traditions. It's a place where shrews whistle commands to beetle workforces, where guinea pig innovations revolutionize ancient farming, where opossums run black markets and raccoons launder money with literal paw-washing.

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>



# Setting Overview for Genesys

The Great Burrow is a **Modern Urban Fantasy** setting with elements of **Steampunk** and **Political Intrigue**. The technology level is roughly equivalent to early 20th century, but adapted for small woodland creatures using natural materials and insect labor instead of electricity and machinery.

**Core Themes:**
- Urban survival in a dangerous world
- Species cooperation vs. traditional hierarchies
- Working-class struggles and economic inequality
- Constant threat from titans and predators
- Community building and mutual aid

## The World Beyond the Walls

### The Titans That Walk
- **Bears**: Could cause total evacuations, physically capable of destroying an entire district
- **Deer**: Their movements reshape landscapes, antler rubs devastate trees
- **Moose**: Rarest but most feared, their feeding can topple ancient oaks
- **Wild Boars**: Their rooting collapses tunnel systems, common and unpredictable

The giants aren't inherently malevolent - they simply exist at a scale that makes coexistence nearly impossible. The Great Burrow has evolved elaborate warning systems, evacuation protocols, and offering stations to minimize catastrophic encounters.

### Natural Predators
- **Hawks**: Control daytime surface travel, forcing covered routes
- **Owls**: Silent death in the night shift
- **Snakes**: Seasonal terror in the canopy
- **Corvids**: Complex relationship - sometimes protection, sometimes threat

\columnbreak

<div class='note'>

#### <u>Scale and Perspective</u>

Understanding scale is crucial in The Great Burrow. A house cat would be a kaiju-level threat. A human footstep could crush entire neighborhoods. The titans - bears, deer, moose - move through the landscape like living natural disasters.

Yet the creatures of The Great Burrow have built a thriving civilization through cooperation, ingenuity, and sheer audacity. This is a world where being small means thinking big.
</div>

\pagebreakNum

## The Five Burrows

### Mousehattan - The Vertical Metropolis
The beating heart of commerce and ambition, carved into a rocky outcropping where ancient oak roots create natural highways. Wall Street is literally carved into walls, while Times Squeak never sleeps under managed firefly lighting. This vertical city rises through seven distinct levels from Sub-Basement to Crown Level, housing 28,000 creatures in a maze of root highways and carved chambers.

**Notable Features:** The Acorn Exchange trading floor built into the Trading Oak's hollow, the Whiskers Building (12 stories of carved stone), Gallery Row displaying rare seeds, and the infamous underground Squeakeasy run by the Longtail crime family. The district operates on "acorn time" with dawn-to-dusk financial markets driving the entire burrow's rhythm.

**Demographics:** 40% mice (old money families), 25% rats (business and crime), 15% voles (middle management), 10% hamsters (merchants), 10% others.

### The Branchx - The Canopy Commons
Working-class pride in three-dimensional tree cities spanning five massive oaks and seven grand maples. 47 major rope bridge crossings connect the vertical neighborhoods, while emergency bark slides provide rapid descent during predator attacks. The canopy stretches across seven branch levels from "Ground Scrape" to "Crown Touch," housing 18,000 creatures in nest complexes and hollow expansions.

**Cultural Identity:** Construction IS The Branchx - from the Nutcracker Union that controls building projects to the rope weavers whose craft passes through generations. The failed tunnel system below serves as both reminder of broken promises and convenient smuggling network. Corvid zones add danger where desperate creatures make deals with crow gangs for aerial protection.

**Demographics:** 60% squirrels (traditional majority), 25% chipmunks (courier class), 10% flying squirrels (premium transport), 5% others including mice gentrifiers.

### The Hives - The Crossroads Community
The Great Burrow's most diverse district, sprawling across meadow clearings where forest meets grassland. This buzzing center of 24,000 creatures earned its name from dense, interconnected burrow complexes honeyccombing the rolling hills. Prairie dog democratic councils share space with traditional rabbit warrens, while guinea pig agricultural terraces demonstrate innovative farming techniques adapted from mountain traditions.

**Economic Hub:** The Great Interchange where three Underground lines converge makes this the logistics capital. 30% of the economy runs on processing external trade, with caravan grounds hosting traders from distant communities. The Sorting Yards warehouse district processes goods from across the forest region, while mixed-species workshops produce fusion crafts combining multiple cultural traditions.

**Cultural Melting Pot:** "Everyone finds their place in the swarm" through cooperation rather than bloodlines. The Integration Center helps newcomers adapt, while cross-cultural families pioneer new ways of living. Night markets buzz with firefly light as creatures enjoy cuisine from across the known world.

### Lin's Brook - The Working Waterfront
Blue-collar waterfront pride where Whisker Creek meets the East River's tidal waters. The Great Dam powers water-driven workshops through Mill Falls, while seven secondary dams create distinct neighborhoods. This engineering marvel houses 20,000 creatures who know that high tide means water work while low tide brings maintenance and repairs.

**Working Culture:** The Dockworkers Union (otter-dominated) shares power with the Builders Guild (beaver-led but increasingly diverse). Traditional industries like sustainable lumber harvesting and fishing feed the entire Great Burrow, while gentrifying Greenbank converts old warehouses into artisanal workshops - to the disgust of working families priced out of their ancestral lodges.

**Water Life:** Complex tail-slap communications coordinate flood protocols for when titans wade through. The Silverclaw crime family controls north dock "protection" while rival otter clans maintain ancient fishing territory disputes. Every kit learns to read currents before they can properly swim.
<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

### Scurry Island - The Forgotten Burrow
Isolated on a true island across dangerous straits, this 10,000-creature community serves as both shadow economy hub and last line of defense against Deep Woods titans. The rocky shores and dense interior provide perfect cover for those seeking to disappear from mainland law. Connected only by three ferries (two usually broken), this is where the desperate, the criminal, and the brave Rangers make their home.

**The Ranger Corps:** Elite scouts operate from fortified Heights overlooking the mainland. Led by a one-eyed badger Watch Commander, they recruit society's desperate to face bears, moose, and worse. Equipment includes poison-tipped porcupine quills, flash powder, and scent bombs. The Wall of the Fallen honors those who stood "between the city and the dark."

**Shadow Economy:** Everything has a price in Harbor Market - from forged documents to concentrated fermented sap. The Fence Lords control major operations while opossum and raccoon families run traditional "businesses." Old Town enforces sanctuary rules even as the Lowland Shanties flood with each storm. Underground fighting pits and gambling dens hide in the Warrens, where "what happens in the deep stays in the deep."



## Infrastructure & Technology

### The Great Underground
The marvel of mole engineering, this subway system connects all five burrows through natural tunnels, hollow logs, and carved passages. Express routes follow main arteries while local service winds through neighborhoods.

**Major Stations:**
- **Grand Central Burrow** (Mousehattan hub)
- **Deep Root & Grove Junction** (The Branchx)
- **The Great Interchange** (The Hives - connects 3 lines)
- **Creek Crossing & Dockside Terminal** (Lin's Brook)
- **Ferry Terminal** (Scurry Island - ferry service only)

Trains are pushed by mole work crews who know every tunnel by vibration. Monthly passes cost 20 acorns, single rides 1-2 acorns depending on distance.

### Communication Networks
- **Tail Signals:** Universal basic communication across species
- **Scent Marking:** Territory boundaries and social status indicators
- **Drumming Networks:** Branch or ground percussion for neighborhood alerts
- **The Daily Squeak:** Newspaper of record (knows what not to print)
- **Chipmunk Couriers:** Rapid message delivery with route-number slang
- **Underground Press:** Radical publications from Village Burrows

### Transportation Methods
Beyond the Underground, creatures navigate via rope bridges (47 major crossings in The Branchx), ferry services (when operational), courier networks, and private options from otter swimming services to rare bat flights. Emergency bark slides provide rapid descent in the canopy, though climbing back up is always harder.

\pagebreakNum

## Economy & Commerce

### The Acorn Standard
Currency valued by quality and preparation method. The Acorn Exchange trading floor in Mousehattan sets prices that ripple across the forest. Seasonal fluctuations drive boom and bust cycles.

**Major Industries by Burrow:**
- **Finance** (Mousehattan): Banking, trading, investment
- **Construction** (The Branchx/Lin's Brook): Infrastructure and building
- **Agriculture** (The Hives): Managed insect operations
- **Fishing/Water Power** (Lin's Brook): Waterfront economy
- **Black Market** (Scurry Island): Shadow economy

### Labor & Unions
- **The Nutcracker Union:** Powerful Branchx construction organization ("we break more than nuts")
- **Dockworkers United:** Lin's Brook waterfront muscle
- **Courier Collectives:** Chipmunk-dominated message services
- **The Builders Guild:** Beaver-led but increasingly diverse

### Economic Status Levels
- **Destitute:** 0-10 acorns (struggling for basic needs)
- **Poor:** 11-50 acorns (working class, paycheck to paycheck)
- **Comfortable:** 51-200 acorns (stable middle class)
- **Wealthy:** 201-1000 acorns (business owners, professionals)
- **Rich:** 1001+ acorns (old money families, crime bosses)

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

## Governance & Politics

### The Five-Burrow Coalition
The Great Burrow operates under a loose confederation where each burrow maintains significant autonomy. The **Inter-Burrow Council** (two representatives per burrow) meets quarterly to handle:
- Infrastructure funding and maintenance
- Titan response coordination
- Inter-burrow dispute resolution
- Trade regulation and standards

The Council cannot override burrow-specific laws or cultural practices.

### Individual Burrow Governance
- **Mousehattan:** Corporate oligarchy run by the Root Board (family heads and crime bosses)
- **The Branchx:** Union democracy through the Nutcracker Assembly with Tail Vote for major decisions
- **The Hives:** Cooperative consensus via the Hive Mind (extended family councils)
- **Lin's Brook:** Guild confederation led by the Dam Council with ancient Water Rights Court
- **Scurry Island:** Survival hierarchy where the Trunk Council maintains order alongside Ranger Command

### Political Movements
- **The Traditionalists:** Preserve burrow autonomy and species-specific governance
- **The Unionists:** Worker rights and cross-species solidarity
- **The Progressives:** Modernization and technological advancement
- **Rangers First:** Titan defense and military preparedness above all
- **The Naturalists:** Environmental protection and sustainable development

\columnbreak

## Historical Context

### The Great Convergence (150 Years Ago)
The city began when multiple crises forced scattered settlements to unite:
- The Terrible Winter (unprecedented cold)
- The Bear Awakening (multiple titan encounters)
- Failed harvests across the forest
- The Great Storm that destroyed isolated communities

The legendary **Acorn Compact** established principles of mutual aid, shared defense, and peaceful dispute resolution that still guide the city.

### Major Historical Events
- **The Species Wars** (76-82 years ago): Economic inequality erupted into inter-species conflict
- **The Great Compromise**: Established current burrow autonomy system
- **The Great Flood** (59 years ago): Demonstrated city's vulnerability and resilience
- **The Great Trampling** (20 years ago): Most destructive titan encounter in city history

### The Modern Era
Recent decades brought unprecedented prosperity alongside new challenges:
- Gentrification displacing traditional communities
- Environmental pressures and increasing titan activity
- Growing wealth inequality testing cooperative spirit
- Immigration from distant forest communities

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

## Daily Life & Culture

### The Rhythm of Survival
- **Dawn:** Highest predator danger, work begins carefully
- **Morning:** Underground commutes, markets open
- **Midday:** Safest surface travel, peak commerce
- **Afternoon:** School, apprenticeships, social time
- **Dusk:** Race to safety, second predator peak
- **Night:** Underground entertainment, black market hours

### Seasonal Pressures
- **Spring:** Flooding threats, mating season tensions
- **Summer:** Tourism peaks, drought stresses water systems
- **Fall:** Harvest determines winter survival
- **Winter:** Food politics dominate, heating becomes currency

### Social Hierarchy
1. **Old Money:** Ancient families with prime territory rights
2. **New Rich:** Entrepreneurs, crime families, innovators
3. **Skilled Workers:** Union members, specialists, guild crafts
4. **Service Class:** Creatures who keep the city running
5. **The Desperate:** Day laborers, refugees, the forgotten

### Crime & Order
Organized families control much of the shadow economy:
- **Mousehattan:** Longtail Family and Whisker Brotherhood
- **Lin's Brook:** Silverclaw Family (waterfront protection)
- **Scurry Island:** Complex black market operations

"Insurance" payments are a fact of life, often providing actual security. The universal code: "The family provides."

\columnbreak

### Cultural Tensions
- **Gentrification:** Old neighborhoods transformed by new money
- **Species Integration:** Young creatures challenging traditional boundaries
- **Innovation vs. Tradition:** Guinea pig methods disrupting rabbit dynasties
- **Height Hierarchies:** Squirrel branch levels determining social status
- **Predator Reality:** Constant threat shapes all architecture and schedules

### Universal Experiences
Every creature knows:
- The Underground commute (packed tunnels, frequent delays)
- Predator drills (alarm signals learned as kits)
- Market days (burrow specialties draw cross-city traffic)
- Weather watching (storms mean infrastructure danger)
- Giant protocols (evacuation procedures when bells ring)

<div class='example'>

##### A Day in The Great Burrow
Maple, a young squirrel construction worker, wakes before dawn in her middle-branch apartment. She checks predator warnings, grabs acorn paste breakfast, and hurries to catch the 6:15 Underground at Grove Junction. 

Packed between commuting beavers and courier chipmunks, she emerges at Deep Root Station to find her crew already assembling. Today they're reinforcing the 42nd Street bridge after yesterday's hawk attack damaged support ropes.

By midday, the bridge is secure. Maple grabs lunch at a mole-run tunnel café, trades gossip about the new guinea pig techniques threatening traditional building methods. Her afternoon is spent in union meetings - the Nutcrackers are organizing against unsafe working conditions on the highest branches.

As dusk approaches, evacuation bells ring - deer sighting near the Grove. Maple and hundreds of others flow into emergency slides, hearts pounding. Safe underground, she joins friends at a root cellar tavern, where tomorrow's worries wash away with fermented berry juice and worker solidarity songs.

This is life in The Great Burrow - dangerous, difficult, but never dull.
</div>

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

# The Shadow Network - Organized Crime

In the shadows between legitimate business and outright banditry lies The Great Burrow's complex criminal underworld. These organizations follow their own codes, respect their own territories, and handle their own justice.

## The Commission

An informal council where major family representatives meet quarterly to resolve disputes and coordinate operations. Meeting locations rotate between neutral territories:
- **Central Crossing** (The Branchx): Bridge intersection for safe meetings
- **The Sanctuary** (Scurry Island): Traditional neutral ground
- **Underground Stations**: Specific platforms with temporary truces

## The Criminal Code

### The Old Laws
1. **Family First**: Blood and chosen family loyalty supersedes all else
2. **Territory Respect**: Honor established boundaries unless formally challenged
3. **No Innocent Blood**: Children, elders, and non-participants are protected
4. **Debt Honor**: Pay what you owe or face escalating consequences
5. **Silence Law**: Never cooperate with outside authorities
6. **Guest Rights**: Sanctuary and safe passage when properly requested

### Criminal Justice
- **Family Courts**: Internal dispute resolution within criminal community
- **Territory Trials**: Formal challenges for boundary disputes
- **Debt Collection**: Escalating pressure from warnings to exile to violence
- **Betrayal Punishment**: Tail cutting, exile, or death depending on severity

## Major Crime Families

### Mousehattan Syndicates
**The Longtail Family** - Traditional Power
- Territory: Waterfront, Wall Street, Times Squeak
- Leadership: Don Salvatore Longtail
- Specialties: Smuggling, financial fraud, loan sharking
- Code: "The family provides"

**The Whisker Brotherhood** - Old Guard
- Territory: Upper levels, residential areas
- Leadership: Council of three brothers
- Specialties: High-end protection, construction permits
- Ritual: Whisker-touching initiation ceremonies

\columnbreak

**The Gray Coats** - Rising Force
- Territory: Village Burrows, young professional areas
- Leadership: Lucia "The Shadow" Gray
- Specialties: Tech fraud, identity theft, blackmail
- Signature: Gray vests marking full members

\pagebreakNum

### Other Burrow Syndicates

**The Silverclaw Family** (Lin's Brook)
- Controls north docks and ferry routes
- Direct violence over subtle manipulation
- Silver-tipped claws worn by made members

**The Honeycomb Family** (The Hives)
- Agricultural mafia controlling honey trade
- Elder Mother Beatrice Honeyclover leads
- Sophisticated commodity manipulation

**The Nutcracker Union** (The Branchx)
- Construction site control and labor intimidation
- Boss Tony "Crack" Nutkin runs operations
- "Worker solidarity" mixed with territorial violence

**The Fence Lords** (Scurry Island)
- Black market masters and document forgers
- Council leadership of proven operators
- "Everything has value to someone"


## Criminal Economics

### Revenue Sources
- **Protection Rackets**: 40% - "Insurance" payments
- **Smuggling**: 25% - Contraband and tax avoidance
- **Gambling**: 15% - Illegal games and fight clubs
- **Labor Control**: 10% - Union corruption
- **Financial Crime**: 10% - Fraud and theft

### Money Laundering
- Legitimate business fronts (restaurants, shops)
- The Washing Circuit (raccoon operations)
- Commodity trading through acorn markets
- Festival economies for cash movement

## Species Specializations

**Rats**: Natural organizers with hierarchical families
**Mice**: Inside operators using respectability
**Raccoons**: Manual dexterity for locks and laundering
**Opossums**: Masters of "playing dead" to authorities
**Beavers**: Infrastructure control and construction corruption
**Otters**: Water smuggling routes and fish market control
**Weasels**: Information brokers and blackmail specialists

<div class='note'>

#### <u>Using Crime in Campaigns</u>

Criminal families provide protection that often includes genuine services - defending against predators, mediating disputes, and economic stabilization. Characters may find themselves needing family help or caught between competing interests.

</div>

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

# Species as Archetypes

Rather than using traditional fantasy races, characters choose from woodland creature species that function as archetypes, each providing different starting characteristics and special abilities.

## The Core Species

### Mice *(The Traditionalists)*

<div class="archetype">
<span class="bra">1</span>
<span class="agi">2</span>
<span class="int">3</span>
<span class="cun">2</span>
<span class="wil">2</span>
<span class="pre">2</span>
</div>

- **Wound Threshold:** 8 + Brawn
- **Strain Threshold:** 12 + Willpower
- **Starting XP:** 100

**Special Abilities:**
- **Tunnel Sense:** Remove <span class='setback'>b</span> from Navigation checks in underground environments
- **Precise Work:** Add <span class='boost'>b</span> to all Mechanics checks
- **Social Networks:** Start with one additional contact in Mousehattan

**Starting Skills:** Choose 2 from: Charm, Deception, Knowledge (City), Mechanics, Negotiation, Streetwise

**Background:** Descendants of the original wall-carvers. Mousehattan IS mouse town in their minds.

**Cultural Traits:**
- Obsessed with genealogy and wall-rights dating back generations
- Believe in "proper" ways of doing everything

**Vocal Patterns:** Precise, articulated speech with old-fashioned vocabulary. Use formal titles and proper grammar even in casual conversation. Speak softly but expect to be heard.

**Occupations:** Bankers, lawyers, Wall Street traders, gallery owners, old-school deli operators

**Species Sayings:**
- *"A mouse can nibble through anything, given time"* (persistence wins)
- *"Know your tunnels, know your exits"* (always have a backup plan)
- *"Cheese ages, roots decay"* (some things improve with time, others don't)

\columnbreak

### Rats *(The Entrepreneurs)*

<div class="archetype">
<span class="bra">2</span>
<span class="agi">2</span>
<span class="int">2</span>
<span class="cun">3</span>
<span class="wil">2</span>
<span class="pre">1</span>
</div>

- **Wound Threshold:** 10 + Brawn
- **Strain Threshold:** 11 + Willpower
- **Starting XP:** 100

**Special Abilities:**
- **Adaptable:** Once per session, may add <span class='boost'>b</span> to any skill check
- **Network Builder:** Reduce difficulty of Streetwise checks by 1 (minimum <span class='ability'>d</span>)
- **Survivor's Instinct:** Add <span class='boost'>b</span> to Vigilance and Cool checks

**Starting Skills:** Choose 2 from: Coercion, Deception, Negotiation, Skulduggery, Streetwise, Vigilance

**Background:** Larger, louder, and less concerned with tradition. They're changing Mousehattan whether the mice like it or not.

**Cultural Traits:**
- "Bigger is better" mentality
- Network aggressively across species lines
- Early adopters of new technology and methods
- Work hard, party harder philosophy

**Vocal Patterns:** Loud, confident speech with lots of emphasis and gesturing. Mix business jargon with street slang. Speak over others and interrupt frequently.

**Occupations:** Tech entrepreneurs, club owners, real estate developers, "import/export"

**Species Sayings:**
- *"Make the hole bigger"* (don't accept limitations)
- *"Every wall's got a weak spot"* (there's always a way)
- *"Swim or sink"* (adapted from ship rat heritage)
- *"The fattest rat gets noticed"* (success makes you a target)

\pagebreakNum

### Squirrels *(The Climbers)*

<div class="archetype">
<span class="bra">2</span>
<span class="agi">3</span>
<span class="int">2</span>
<span class="cun">2</span>
<span class="wil">1</span>
<span class="pre">2</span>
</div>

- **Wound Threshold:** 9 + Brawn
- **Strain Threshold:** 10 + Willpower
- **Starting XP:** 100

**Special Abilities:**
- **Arboreal Movement:** Ignore difficult terrain when climbing, add <span class='boost'>b</span> to Athletics (climbing) checks
- **Territorial Instinct:** Add <span class='boost'>b</span> to Vigilance checks in familiar territory
- **Hoarder's Memory:** Add <span class='boost'>b</span> to Knowledge checks about valuable items

**Starting Skills:** Choose 2 from: Athletics, Coordination, Perception, Survival, Vigilance, Knowledge (City)

**Background:** Traditional Branchx residents, multi-generational canopy builders.

**Cultural Traits:** Height hierarchy obsessed, natural hoarders, territorial about acorn groves, master rope bridge builders.

**Vocal Patterns:** Quick, clipped speech with dropped consonants when excited. Tree cluster accents vary by neighborhood.

**Occupations:** Construction, bridge building, union organizing, canopy police

**Sayings:** *"High branch, warm winter"* / *"Never trust a ground-dweller with your nuts"*

\columnbreak

### Chipmunks *(The Couriers)*

<div class="archetype">
<span class="bra">1</span>
<span class="agi">3</span>
<span class="int">2</span>
<span class="cun">2</span>
<span class="wil">2</span>
<span class="pre">2</span>
</div>

- **Wound Threshold:** 8 + Brawn
- **Strain Threshold:** 11 + Willpower
- **Starting XP:** 100

**Special Abilities:**
- **Speed Burst:** Once per encounter, may move to any location within Medium range as an incidental
- **Cheek Pouches:** Can carry small items without encumbrance penalty
- **Route Knowledge:** Remove <span class='setback'>b</span> from Streetwise checks related to navigation

**Starting Skills:** Choose 2 from: Athletics, Coordination, Perception, Vehicles, Streetwise, Vigilance

**Background:** Fast Branchx couriers, risk-takers who form tight crew families.

**Cultural Traits:** Speed obsessed, proud of cheek-pouch capacity, route efficiency focused, crew loyalty over height status.

**Vocal Patterns:** Rapid-fire delivery with slang and abbreviations. Extensive hand gestures, crew members finish each other's sentences.

**Occupations:** Messengers, couriers, smugglers, tunnel maintenance

**Sayings:** *"Full cheeks, empty promises"* / *"Winter comes for the slow"*

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

### Beavers *(The Builders)*

<div class="archetype">
<span class="bra">3</span>
<span class="agi">1</span>
<span class="int">2</span>
<span class="cun">2</span>
<span class="wil">2</span>
<span class="pre">2</span>
</div>

- **Wound Threshold:** 12 + Brawn
- **Strain Threshold:** 11 + Willpower
- **Starting XP:** 100

**Special Abilities:**
- **Master Builder:** Add <span class='boost'>b</span> to all Mechanics checks involving construction
- **Aquatic:** Can hold breath for extended periods, swim at full speed
- **Sturdy:** Increase soak value by 1

**Starting Skills:** Choose 2 from: Athletics, Mechanics, Knowledge (Science), Resilience, Survival, Vigilance

**Background:** Premier infrastructure species, Lin's Brook dam and lodge builders.

**Cultural Traits:** Judge by work quality, suspicious of "artisanal" trends, generational lodges, practical problem-solving pride.

**Vocal Patterns:** Methodical construction terminology, measured engineering explanations, building and water metaphors.

**Occupations:** Dam building, construction, water management, lumber processing

**Sayings:** *"Busy as a beaver"* / *"Still water, strong dam"*


### Rabbits *(The Cooperators)*

<div class="archetype">
<span class="bra">2</span>
<span class="agi">2</span>
<span class="int">1</span>
<span class="cun">2</span>
<span class="wil">2</span>
<span class="pre">3</span>
</div>

- **Wound Threshold:** 10 + Brawn
- **Strain Threshold:** 11 + Willpower
- **Starting XP:** 110

**Special Abilities:**
- **Community Bonds:** Add <span class='boost'>b</span> to Leadership and Charm checks
- **Danger Sense:** Add <span class='boost'>b</span> to Initiative checks
- **Large Family:** Start with additional family contacts

**Starting Skills:** Choose 2 from: Charm, Knowledge (Science), Leadership, Medicine, Negotiation, Survival

**Background:** Master beekeepers controlling honey trade through family operations.

**Cultural Traits:** Wealth measured in hives, large families as status, protective of trade secrets, expert warren diggers.

**Vocal Patterns:** Warm agricultural metaphors, collective family terms, diminutives and endearments.

**Occupations:** Beekeeping, honey trade, warren architecture, garden design

**Sayings:** *"Breed like rabbits, work like bees"* / *"Every kit needs a warren"*

### Guinea Pigs *(The Innovators)*

<div class="archetype">
<span class="bra">1</span>
<span class="agi">2</span>
<span class="int">2</span>
<span class="cun">2</span>
<span class="wil">2</span>
<span class="pre">3</span>
</div>

- **Wound Threshold:** 8 + Brawn
- **Strain Threshold:** 11 + Willpower
- **Starting XP:** 110

**Special Abilities:**
- **Community Minded:** Add <span class='boost'>b</span> to Leadership checks
- **Insect Whisperer:** Add <span class='boost'>b</span> to Animal Handling checks with insects
- **Mountain Heritage:** Add <span class='boost'>b</span> to Survival checks in difficult terrain

**Starting Skills:** Choose 2 from: Animal Handling, Knowledge (Science), Leadership, Medicine, Survival, Charm

**Background:** Mountain immigrants bringing revolutionary terracing and communal traditions.

**Cultural Traits:** Group decision-making through squeaking councils, beetle-communication whistlers, mountain-to-forest adaptation specialists.

**Vocal Patterns:** Musical speech with rolling R's, Common Forest/Andean dialect switching, collective "we" instead of "I."

**Occupations:** Agricultural consulting, terrace engineering, textile weaving, beetle-whispering

**Sayings:** *"The mountain remembers"* / *"Whistle while you work"*

<div class='example'>

##### Character Creation Example
Pip is creating a mouse character. She takes the mouse archetype (Brawn 1, Agility 2, Intellect 3, Cunning 2, Willpower 2, Presence 2) and decides to play an up-and-coming trader from Mousehattan. She chooses Charm and Negotiation as her starting skills and takes the Acorn Trader career for additional business skills.
</div>

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

# Additional Species


### Otters *(The Watercreatures)*

<div class="archetype">
<span class="bra">2</span>
<span class="agi">3</span>
<span class="int">1</span>
<span class="cun">2</span>
<span class="wil">2</span>
<span class="pre">2</span>
</div>

- **Wound Threshold:** 10 + Brawn
- **Strain Threshold:** 11 + Willpower  
- **Starting XP:** 100

**Special Abilities:**
- **Aquatic Excellence:** Add <span class='boost'>b</span><span class='boost'>b</span> to all swimming checks, hold breath for extended periods
- **Playful Competitor:** Add <span class='boost'>b</span> to Cool checks during stressful social situations
- **Water Sense:** Remove <span class='setback'>b</span> from Navigation checks near water

**Starting Skills:** Choose 2 from: Athletics, Coordination, Charm, Perception, Survival, Vehicles

**Background:** Lin's Brook fishers and waterfront workers with playful-but-serious work ethic.

**Cultural Traits:** Competitive family groups, natural swimmers, competitive sliding, pity "dry-landers."

**Vocal Patterns:** Water metaphors, overlapping conversations, playful competitive banter.

**Occupations:** Fishing, dock work, ferry operations, swimming instruction

**Sayings:** *"Slick as an otter's slide"* / *"Fish don't catch themselves"*

### Opossums *(The Survivors)*

<div class="archetype">
<span class="bra">2</span>
<span class="agi">2</span>
<span class="int">2</span>
<span class="cun">3</span>
<span class="wil">2</span>
<span class="pre">1</span>
</div>

- **Wound Threshold:** 10 + Brawn
- **Strain Threshold:** 11 + Willpower
- **Starting XP:** 100

**Special Abilities:**
- **Play Dead:** Once per session, end engagement by feigning death
- **Scavenger's Eye:** Add <span class='boost'>b</span> to Perception for useful items
- **Nocturnal:** Remove <span class='setback'>b</span> from checks in darkness

\columnbreak

**Starting Skills:** Choose 2 from: Deception, Skulduggery, Streetwise, Survival, Vigilance, Cool

**Background:** Shadow economy masters using "play dead" philosophy.

**Cultural Traits:** Nocturnal adaptation specialists, dark humor, "less than you are" philosophy.

**Vocal Patterns:** Drawling speech turning sharp, folksy sayings, quiet forcing others to lean in.

**Occupations:** Black market, night work, scavenging, "problem solving"

**Sayings:** *"Play dead 'til you're ready"* / *"Every garbage got treasure"*


### Raccoons *(The Operators)*

<div class="archetype">
<span class="bra">2</span>
<span class="agi">3</span>
<span class="int">2</span>
<span class="cun">3</span>
<span class="wil">1</span>
<span class="pre">1</span>
</div>

- **Wound Threshold:** 10 + Brawn
- **Strain Threshold:** 10 + Willpower
- **Starting XP:** 90

**Special Abilities:**
- **Nimble Fingers:** Add <span class='boost'>b</span><span class='boost'>b</span> to manual Skulduggery
- **Mask of Innocence:** Add <span class='boost'>b</span> to innocent Deception
- **Washing Ritual:** "Clean" stolen goods, reduce selling difficulty by 1

**Starting Skills:** Choose 2 from: Deception, Skulduggery, Streetwise, Coordination, Vigilance, Negotiation

**Background:** Scurry Island black market operators and money launderers.

**Cultural Traits:** Literal/metaphorical washing, dexterity pride, loose "ring" families, legal/illegal navigation.

**Vocal Patterns:** Smooth persuasion with hand gestures, code-switching, constant euphemisms.

**Occupations:** Smuggling, fence operations, lock "specialization," legitimate fronts

**Sayings:** *"Clean paws, dirty deals"* / *"Five fingers, five opportunities"*

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

### Badgers *(The Old Guard)*

<div class="archetype">
<span class="bra">4</span>
<span class="agi">1</span>
<span class="int">2</span>
<span class="cun">2</span>
<span class="wil">3</span>
<span class="pre">2</span>
</div>

- **Wound Threshold:** 14 + Brawn
- **Strain Threshold:** 12 + Willpower
- **Starting XP:** 90

**Special Abilities:**
- **Territorial Defender:** Add <span class='boost'>b</span><span class='boost'>b</span> when defending property
- **Intimidating Presence:** Add <span class='boost'>b</span> to Coercion
- **Ancient Rights:** Start with inherited property/land rights

**Starting Skills:** Choose 2 from: Brawl, Coercion, Knowledge (City), Negotiation, Resilience, Vigilance

**Background:** Pre-city ancient families owning prime land, viewing others as newcomers.

**Cultural Traits:** Territorial traditionalists, fortress-like ancestral burrows, physical dispute resolution, suspicious of "city ways."

**Vocal Patterns:** Gruff old-fashioned vocabulary, short declarative sentences, territorial metaphors.

**Occupations:** Landlords, old-money investment, traditional crafts, dispute mediation

**Sayings:** *"The burrow remembers"* / *"Claw law"*


### Prairie Dogs *(The Democrats)*

<div class="archetype">
<span class="bra">2</span>
<span class="agi">2</span>
<span class="int">2</span>
<span class="cun">2</span>
<span class="wil">2</span>
<span class="pre">3</span>
</div>

- **Wound Threshold:** 10 + Brawn
- **Strain Threshold:** 11 + Willpower
- **Starting XP:** 100

**Special Abilities:**
- **Democratic Process:** Add <span class='boost'>b</span><span class='boost'>b</span> to group Leadership
- **Early Warning:** Add <span class='boost'>b</span> to Initiative and danger Vigilance
- **Community Organizer:** Reduce group social check difficulty by 1

**Background:** Grassland immigrants bringing democratic traditions and community organization.

**Cultural Traits:** Complex democratic processes, collective action believers, early warning specialists.

**Vocal Patterns:** Clear projected speech, collective pronouns, organized turn-taking.

**Occupations:** Community organizing, democratic facilitation, grain processing, logistics

**Sayings:** *"The burrow decides together"* / *"Many voices, clear choice"*


### Marmots *(The Craftscreatures)*

<div class="archetype">
<span class="bra">3</span>
<span class="agi">1</span>
<span class="int">3</span>
<span class="cun">2</span>
<span class="wil">2</span>
<span class="pre">1</span>
</div>

- **Wound Threshold:** 12 + Brawn
- **Strain Threshold:** 11 + Willpower
- **Starting XP:** 100

**Special Abilities:**
- **Mountain Wisdom:** Add <span class='boost'>b</span> to geology/weather Knowledge
- **Master Craftscreature:** Add <span class='boost'>b</span><span class='boost'>b</span> to stone/mineral Mechanics
- **Seasonal Awareness:** Add <span class='boost'>b</span> to Survival

**Background:** Highland immigrants with stone-working expertise and alpine survival traditions.

**Cultural Traits:** Stone/mineral specialists, seasonal awareness, multi-generational knowledge, quality over speed values.

**Vocal Patterns:** Technical precision, geological terminology, patient stone-worker speech.

**Occupations:** Stone work, mineral processing, weather prediction, construction specialization

**Sayings:** *"Stone remembers the mountain"* / *"Slow chisel, strong foundation"*

### Moles *(The Underground Elite)*

<div class="archetype">
<span class="bra">2</span>
<span class="agi">1</span>
<span class="int">3</span>
<span class="cun">3</span>
<span class="wil">2</span>
<span class="pre">1</span>
</div>

- **Wound Threshold:** 10 + Brawn
- **Strain Threshold:** 11 + Willpower
- **Starting XP:** 100

**Special Abilities:**
- **Underground Navigation:** Remove <span class='setback'>b</span><span class='setback'>b</span> from underground Navigation
- **Tremor Sense:** Add <span class='boost'>b</span><span class='boost'>b</span> to vibration Perception
- **Tunnel Vision:** Upgrade visual Perception difficulty by 1, immune to visual distractions

**Background:** Subway operators building and maintaining the Great Underground.

**Cultural Traits:** Touch/sound navigation, soil quality obsession, vibration crew communication, wealthy from transit monopoly.

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

**Vocal Patterns:** Quiet technical speech, no direct eye contact, tactile/auditory descriptions.

**Occupations:** Subway operation, tunnel engineering, underground police, soil analysiss

**Sayings:** *"Dig deep, breathe shallow"*



### Skunks *(The Enforcers)*

<div class="archetype">
<span class="bra">3</span>
<span class="agi">2</span>
<span class="int">2</span>
<span class="cun">2</span>
<span class="wil">3</span>
<span class="pre">2</span>
</div>

- **Wound Threshold:** 12 + Brawn
- **Strain Threshold:** 12 + Willpower
- **Starting XP:** 90

**Special Abilities:**
- **Chemical Defense:** Once per encounter, Short range creatures make Average <span class='difficulty'>d</span><span class='difficulty'>d</span> Resilience or Staggered 2 rounds
- **Intimidating Reputation:** Add <span class='boost'>b</span><span class='boost'>b</span> to Coercion
- **Calm Authority:** Add <span class='boost'>b</span> to Cool and Leadership

**Background:** Natural defense mechanism parlayed into security and enforcement careers.

**Cultural Traits:** Confident from spray defense, tight families, sophisticated dress, pride in restraint.

**Vocal Patterns:** Calm measured speech commanding attention, precise language, no ambiguity.

**Occupations:** Security, bodyguards, waste management, chemical processing

**Sayings:** *"Lift the tail, end the tale"* / *"Black and white, clear as night"*

### Ferrets *(The Dealers)*

<div class="archetype">
<span class="bra">1</span>
<span class="agi">4</span>
<span class="int">2</span>
<span class="cun">3</span>
<span class="wil">1</span>
<span class="pre">3</span>
</div>

- **Wound Threshold:** 8 + Brawn
- **Strain Threshold:** 10 + Willpower
- **Starting XP:** 90

**Special Abilities:**
- **Hyperactive:** May perform 1 additional maneuver per turn without strain cost
- **Deal Maker:** Add <span class='boost'>b</span> to Negotiation and Streetwise checks
- **Flexible:** Add <span class='boost'>b</span> to Coordination checks involving squeezing through spaces

**Starting Skills:** Choose 2 from: Coordination, Negotiation, Streetwise, Charm, Skulduggery, Perception

\columnbreak

**Background:** Hyperactive deal-makers who thrive in the city's fast pace. Natural middlemen.

**Cultural Traits:**
- Can't sit still, always working multiple angles
- Form business "kits" rather than traditional families
- Obsessive collectors of shiny objects
- Dance through legal grey areas

**Vocal Patterns:** Extremely rapid speech that jumps between topics. Use lots of slang and made-up words. Speak with infectious enthusiasm about everything.

**Occupations:** Brokers, messengers, fences, entertainment promoters, "consultants"

**Species Sayings:**
- *"War dance first, negotiate later"* (intimidation tactics)
- *"If it shines, it's mine"* (everything has value)
- *"Sleep when you're dead"* (constant motion)
- *"Slip through, slide by"* (flexibility is key)


### Porcupines *(The Artists)*

<div class="archetype">
<span class="bra">3</span>
<span class="agi">1</span>
<span class="int">3</span>
<span class="cun">2</span>
<span class="wil">3</span>
<span class="pre">2</span>
</div>

- **Wound Threshold:** 12 + Brawn
- **Strain Threshold:** 12 + Willpower
- **Starting XP:** 90

**Special Abilities:**
- **Quill Defense:** When attacked in melee, attacker suffers 1 strain (2 strain on critical hit)
- **Artistic Vision:** Add <span class='boost'>b</span><span class='boost'>b</span> to checks involving artistic creation
- **Defensive Stance:** Add <span class='boost'>b</span> to defense when not moving

**Starting Skills:** Choose 2 from: Cool, Discipline, Mechanics, Medicine, Perception, Knowledge (City)

**Background:** Natural armor makes them perfect guards, but they're tired of being typecast.

**Cultural Traits:**
- Constantly fighting "all quills, no brains" stereotype
- Actually quite artistic and philosophical
- Form collective artist communities
- Use shed quills for various crafts

**Vocal Patterns:** Thoughtful, deliberate speech with artistic vocabulary. Often pause mid-sentence to consider their words carefully. Use lots of metaphors about protection and vulnerability.

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

**Occupations:** Guards, artists, quill-crafters, acupuncturists, philosophers

**Species Sayings:**
- *"Quills out, walls up"* (defensive stance)
- *"Every point has a purpose"* (nothing is without meaning)
- *"Back off means back off"* (clear boundaries)
- *"Soft belly, sharp back"* (vulnerability and strength)



### Weasels *(The Information Brokers)*

<div class="archetype">
<span class="bra">1</span>
<span class="agi">3</span>
<span class="int">2</span>
<span class="cun">4</span>
<span class="wil">2</span>
<span class="pre">2</span>
</div>

- **Wound Threshold:** 8 + Brawn
- **Strain Threshold:** 11 + Willpower
- **Starting XP:** 90

**Special Abilities:**
- **Information Network:** Once per session, may know a useful rumor or secret
- **Serpentine Movement:** Add <span class='boost'>b</span><span class='boost'>b</span> to Stealth and Coordination checks in tight spaces
- **Social Chameleon:** Add <span class='boost'>b</span> to Deception checks when mimicking social groups

**Starting Skills:** Choose 2 from: Deception, Perception, Skulduggery, Streetwise, Vigilance, Charm

**Background:** The gossips, spies, and information dealers who know everyone's business.

**Cultural Traits:**
- Incredibly flexible, physically and morally
- Trade in secrets more than goods
- Form loose networks rather than families
- Can literally get into anywhere

**Vocal Patterns:** Smooth, insinuating speech that draws others into conversation. Masters of asking leading questions. Use lots of euphemisms and coded language.

**Occupations:** Spies, journalists, private investigators, couriers, bartenders

**Species Sayings:**
- *"Weasel in, truth out"* (we find what's hidden)
- *"Every hole has a secret"* (information is everywhere)
- *"Bend don't break"* (adaptability is survival)
- *"Pop goes the weasel"* (sudden revelations)


\columnbreak

### Groundhogs *(The Bureaucrats)*

<div class="archetype">
<span class="bra">2</span>
<span class="agi">1</span>
<span class="int">3</span>
<span class="cun">2</span>
<span class="wil">3</span>
<span class="pre">2</span>
</div>

- **Wound Threshold:** 10 + Brawn
- **Strain Threshold:** 12 + Willpower
- **Starting XP:** 100

**Special Abilities:**
- **Weather Prediction:** Add <span class='boost'>b</span><span class='boost'>b</span> to checks related to predicting weather or seasonal changes
- **Bureaucratic Procedure:** Add <span class='boost'>b</span> to Knowledge (City) checks involving regulations or paperwork
- **Seasonal Slow:** During winter months, upgrade difficulty of Athletics checks by 1 but gain <span class='boost'>b</span> to all mental skills

**Starting Skills:** Choose 2 from: Knowledge (City), Knowledge (Science), Negotiation, Perception, Cool, Discipline

**Background:** Their weather prediction tradition evolved into complex bureaucratic roles.

**Cultural Traits:**
- Obsessed with patterns and predictions
- Natural bureaucrats who love paperwork
- Hibernate partially, leading to seasonal government slowdowns
- Take their shadow-seeing traditions VERY seriously

**Vocal Patterns:** Formal, bureaucratic speech with lots of qualifiers and subclauses. Speak in official terminology even in casual conversation. Use weather metaphors for everything.


**Occupations:** Bureaucrats, weather predictors, record keepers, seasonal planners

**Species Sayings:**
- *"Six more weeks"* (delays are inevitable)
- *"Check your shadow"* (examine yourself)
- *"Forms in triplicate"* (proper procedure matters)
- *"Spring comes when it comes"* (patience with natural cycles)

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

### Bats *(The Night Shift)*

<div class="archetype">
<span class="bra">1</span>
<span class="agi">4</span>
<span class="int">2</span>
<span class="cun">3</span>
<span class="wil">2</span>
<span class="pre">2</span>
</div>

- **Wound Threshold:** 8 + Brawn
- **Strain Threshold:** 11 + Willpower
- **Starting XP:** 100

**Special Abilities:**
- **Echolocation:** Remove <span class='setback'>b</span><span class='setback'>b</span> from Perception checks in darkness, add <span class='boost'>b</span> to Navigation checks
- **Flight:** Can fly at speed 2, ignoring terrain
- **Night Vision:** Remove <span class='setback'>b</span> from all checks made in darkness

**Starting Skills:** Choose 2 from: Perception, Navigation, Vehicles, Cool, Vigilance, Athletics

**Background:** The only flying mammals, they dominate nighttime aerial courier and reconnaissance work.

**Cultural Traits:**
- Echolocation gives them unique perspective
- Form massive colonies but value individual achievement
- Bridge the gap between ground and canopy
- Mysterious reputation they cultivate

**Vocal Patterns:** High-pitched, precise speech with excellent diction. Often speak in technical terms about navigation and acoustics. Use lots of spatial and directional language.

**Occupations:** Night couriers, aerial reconnaissance, night doctors, sound engineers

**Species Sayings:**
- *"Blind as a bat"* (said sarcastically - they see everything)
- *"Hang together or fall alone"* (community matters)
- *"Echo tells truth"* (listen more than you speak)
- *"Night flight, day fright"* (own your time)

\columnbreak

### Foxes *(The Cunning Outcasts)*

<div class="archetype">
<span class="bra">2</span>
<span class="agi">3</span>
<span class="int">4</span>
<span class="cun">4</span>
<span class="wil">2</span>
<span class="pre">1</span>
</div>

- **Wound Threshold:** 10 + Brawn
- **Strain Threshold:** 11 + Willpower
- **Starting XP:** 80

**Special Abilities:**
- **Cunning Hunter:** Add <span class='boost'>b</span><span class='boost'>b</span> to Skulduggery and Deception checks
- **Predator Heritage:** Must make Hard <span class='difficulty'>d</span><span class='difficulty'>d</span><span class='difficulty'>d</span> Discipline check when around small creatures to avoid intimidating them
- **Quick Thinking:** Once per session, upgrade any skill check twice instead of once

**Starting Skills:** Choose 2 from: Deception, Skulduggery, Negotiation, Cool, Perception, Knowledge (City)

**Background:** Usually predators, but some have chosen to integrate into society. Never fully trusted.

**Cultural Traits:**
- Must constantly prove their "civilized" status
- Often the smartest creature in the room
- Natural loners who struggle with city life
- Use their reputation strategically

**Vocal Patterns:** Articulate, careful speech that sounds almost too polished. Use sophisticated vocabulary to prove their intelligence. Speak with slight hesitation, choosing words carefully.

**Occupations:** Lawyers, negotiators, private investigators, problem solvers

**Species Sayings:**
- *"Trust a fox to be a fox"* (nature is nature)
- *"Every chicken has my name on it"* (fighting instincts)
- *"Clever is as clever does"* (prove your worth)
- *"Hunt alone, live alone"* (independence has a price)

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

\pagebreakNum

### Dogs *(The Loyal Companions)*

<div class="archetype">
<span class="bra">3</span>
<span class="agi">2</span>
<span class="int">1</span>
<span class="cun">2</span>
<span class="wil">3</span>
<span class="pre">3</span>
</div>

- **Wound Threshold:** 12 + Brawn
- **Strain Threshold:** 12 + Willpower
- **Starting XP:** 100

**Special Abilities:**
- **Pack Loyalty:** Add <span class='boost'>b</span><span class='boost'>b</span> to checks when helping allies or defending family
- **Enhanced Senses:** Add <span class='boost'>b</span> to Perception checks using smell or hearing
- **Wolf Heritage:** May cause fear in other creatures; once per session, add <span class='boost'>b</span> to Coercion checks

**Starting Skills:** Choose 2 from: Athletics, Cool, Leadership, Perception, Vigilance, Discipline

**Background:** Rare but valued members of society, dogs carry the burden of being distant cousins to the titan Wolves.

**Cultural Traits:**
- Intensely loyal to chosen families and communities
- Natural protectors with strong territorial instincts
- Struggle with their reputation due to wolf heritage
- Form tight pack bonds with other species

**Vocal Patterns:** Warm, earnest speech with pack-oriented language. Use lots of loyalty and family metaphors. Speak with conviction and sincerity.

**Occupations:** Security guards, family protectors, emotional support workers, community mediators, search and rescue

**Species Sayings:**
- *"Pack first, self second"* (loyalty above all)
- *"A good nose knows"* (trust your instincts)
- *"Howl with the family, hunt with the pack"* (different roles for different groups)
- *"The wolf's shadow doesn't define the dog"* (you are not your ancestors)

\columnbreak

### Cats *(The Independent Observers)*

<div class="archetype">
<span class="bra">1</span>
<span class="agi">4</span>
<span class="int">3</span>
<span class="cun">3</span>
<span class="wil">3</span>
<span class="pre">2</span>
</div>

- **Wound Threshold:** 8 + Brawn
- **Strain Threshold:** 12 + Willpower
- **Starting XP:** 90

**Special Abilities:**
- **Feline Reflexes:** Add <span class='boost'>b</span><span class='boost'>b</span> to Initiative and Coordination checks
- **Night Hunter:** Remove <span class='setback'>b</span> from Stealth and Perception checks in low light
- **Independent:** Add <span class='boost'>b</span> to checks made when working alone

**Starting Skills:** Choose 2 from: Stealth, Perception, Cool, Coordination, Vigilance, Skulduggery

**Background:** Sophisticated and somewhat aloof, cats maintain their independence while participating in city life.

**Cultural Traits:**
- Fiercely independent but capable of deep loyalty
- Natural hunters with excellent night vision and reflexes
- Maintain dignity and composure in most situations
- Form selective social bonds rather than broad communities

**Vocal Patterns:** Precise, measured speech with careful word choice. Use hunting and territory metaphors. Speak quietly but expect to be heard.

**Occupations:** Private investigators, night watchmen, independent contractors, mediators, quality inspectors

**Species Sayings:**
- *"Nine lives, one purpose"* (resilience with focus)
- *"The mouse reveals the maze"* (small details show big patterns)
- *"Hunt alone, sleep together"* (independence and companionship both matter)
- *"Not all who prowl are predators"* (don't judge by appearance)


<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

### Shrews *(The Insect Whisperers)*

<div class="archetype">
<span class="bra">1</span>
<span class="agi">2</span>
<span class="int">2</span>
<span class="cun">2</span>
<span class="wil">1</span>
<span class="pre">2</span>
</div>

- **Wound Threshold:** 8 + Brawn
- **Strain Threshold:** 8 + Willpower
- **Starting XP:** 110

**Special Abilities:**
- **Insect Communication:** Can communicate with insects through ultrasonic whistles, add <span class='boost'>b</span><span class='boost'>b</span> to Animal Handling checks with insects
- **Hyperactive Metabolism:** Must eat every 4 hours or suffer strain, but add <span class='boost'>b</span> to Athletics checks
- **Tiny Size:** Add <span class='boost'>b</span><span class='boost'>b</span> to Stealth checks, but increase difficulty of Brawl checks by 1

**Starting Skills:** Choose 2 from: Animal Handling, Knowledge (Science), Survival, Perception, Medicine, Mechanics

**Background:** The smallest mammals with the biggest appetites and the unique ability to communicate with beetles and other insects.

**Cultural Traits:**
- Metabolisms so fast they're always eating or working
- Each family has unique whistle-patterns passed down generations
- Natural partnerships with beetle colonies they see as extended family

**Vocal Patterns:** Extremely rapid, high-pitched speech that sounds almost like squeaking to larger creatures. Often whistle while talking, creating complex layered communication.

**Occupations:** Beetle herders, insect behavioral specialists, composting managers, pest negotiators

**Species Sayings:**
- *"A beetle knows an honest whistle"* (truth is recognized)
- *"Fast heart, faster hands"* (speed in everything)
- *"You can't rush good compost"* (quality takes time)
- *"Hungry shrew, busy shrew"* (necessity drives work)

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

### Voles *(The Middle Managers)*

<div class="archetype">
<span class="bra">2</span>
<span class="agi">2</span>
<span class="int">2</span>
<span class="cun">2</span>
<span class="wil">2</span>
<span class="pre">2</span>
</div>

- **Wound Threshold:** 9 + Brawn
- **Strain Threshold:** 11 + Willpower
- **Starting XP:** 110

**Special Abilities:**
- **Reliable Workers:** Once per session, may reroll any failed skill check
- **Administrative Mind:** Add <span class='boost'>b</span> to all Knowledge checks related to bureaucracy or organization
- **Unnoticed:** Often overlooked, add <span class='boost'>b</span> to Stealth checks in social situations

**Starting Skills:** Choose 2 from: Knowledge (City), Negotiation, Perception, Vigilance, Discipline, Cool

**Background:** The backbone of Mousehattan's service economy, voles keep the city running through quiet competence and administrative expertise.

**Cultural Traits:**
- Masters of middle management and bureaucratic systems
- Excellent at remembering details and following procedures
- Often underestimated but essential to city operations
- Strong work ethic with emphasis on reliability over ambition

**Vocal Patterns:** Measured, professional speech with careful word choice. Tend to speak in passive voice and use qualifying statements. Never interrupt superiors.


### Hamsters *(The Hoarders)*

<div class="archetype">
<span class="bra">2</span>
<span class="agi">1</span>
<span class="int">2</span>
<span class="cun">3</span>
<span class="wil">2</span>
<span class="pre">2</span>
</div>

- **Wound Threshold:** 10 + Brawn
- **Strain Threshold:** 11 + Willpower
- **Starting XP:** 100

**Special Abilities:**
- **Cheek Pouches:** Can carry items up to Encumbrance 3 without penalty
- **Storage Expert:** Add <span class='boost'>b</span><span class='boost'>b</span> to checks involving organizing or finding stored items
- **Hibernation Heritage:** Can survive on minimal resources, reduce lifestyle costs by 50%

**Starting Skills:** Choose 2 from: Negotiation, Knowledge (City), Mechanics, Perception, Vigilance, Survival

**Background:** Natural merchants and storage specialists, hamsters run many of Mousehattan's warehouses and trading posts.

**Cultural Traits:**
- Obsessive about storage and organization systems
- Natural traders with excellent memory for inventory
- Tendency to prepare for worst-case scenarios
- Strong family businesses passed through generations

**Vocal Patterns:** Slightly muffled speech (cheek pouches), rapid listing of items and prices. Excel at mental mathematics and speak in merchant shorthand.

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

## Cultural Notes for Game Masters

### Mixed Heritage and Adoption

Cross-species relationships have become increasingly common in The Great Burrow's urban environment. These relationships face both social challenges and practical considerations.

**Common Pairings:**
- Mouse-Rat families often bridge old money and new money cultures
- Squirrel-Chipmunk partnerships share canopy lifestyle but different approaches
- Beaver-Otter couples share aquatic focus but different work philosophies
- Rabbit-Guinea Pig families create strong agricultural cooperation bonds

**Mixed-Heritage Children:**
- Are physically one parent's species but may show subtle influences from both
- Often create new traditions blending both parents' backgrounds
- May face acceptance issues from traditional communities
- Natural bridge-builders between different species communities

### Regional and Class Variations

**Urban vs. Rural Differences:**
- City Mice: Sophisticated, formal, focused on finance and precision
- Rural Mice: More practical, less formal, focused on traditional crafts
- Dock Rats vs. Business Rats: Different values around risk and cooperation
- Canopy vs. Ground Squirrels: Ongoing tensions over status and resources

### Vocal Pattern Guidelines for Roleplay

**NYC Cultural Influences:**
- Working Class: Chipmunks, squirrels, beavers, otters reflect NYC working-class speech
- Business/Professional: Mice, rats, some rabbits show professional communication
- Immigrant Communities: Guinea pigs represent code-switching speech patterns
- Neighborhood Variations: Each burrow has distinct local speech patterns

\columnbreak

**General Guidelines:**
- Species provide baseline tendencies, but individual variation is common
- Neighborhood and occupation often influence speech more than species
- Younger creatures have more mixed speech patterns from inter-species contact
- Stress can cause creatures to revert to more species-typical patterns

<div class='note'>

#### <u>Species Longevity and Lifecycle</u>

Different species have varying lifespans that affect career planning and social dynamics:

**Short-lived Species (6-10 years):** Mice, rats - fast-paced lives with intense focus

**Medium-lived Species (10-16 years):** Squirrels, rabbits, guinea pigs - long-term planning

**Long-lived Species (30-40 years):** Beavers, badgers - extensive institutional memory

This creates intergenerational dynamics where longer-lived species serve as mentors and institutional memory, while shorter-lived species drive innovation and change.

</div>

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

# The Five Burrows - Detailed Guide

Each burrow has its own distinct character, challenges, and opportunities. Understanding the neighborhoods and notable locations helps bring The Great Burrow to life.

## Mousehattan - The Vertical Metropolis

### Districts

#### Wall Street (Financial District)
Literally carved into the main rock wall beneath the Trading Oak, this is the economic heart of The Great Burrow.
- **The Acorn Exchange Trading Floor**: Inside the Trading Oak's hollow, sets prices forest-wide
- **Root Vaults**: Ancient storage chambers where old families keep their wealth
- **Counting Rooms**: Traditional notched-stick tallying systems still in use
- **Grove Rights Office**: Where oak territory ownership is registered

#### Times Squeak (Entertainment District)
Where five major tunnels converge beneath interlocking roots, buzzing with 24-hour activity.
- **Firefly Lantern District**: Managed colonies provide atmospheric lighting
- **The Squeak**: Famous performance venue for death theater and comedy
- **Roasted Seed Row**: Street vendors selling traditional and fusion snacks
- **The Moonlight Market**: After-hours trading in "fell off the tree" goods

#### Upper East Roots (Old Money Residential)
Carved into the most stable oak root systems, home to established families.
- **The Acorn Club**: Exclusive social organization requiring 5-generation membership
- **Gallery Row**: Displaying rare seeds, pressed leaves, and natural art
- **Private Warren Entrances**: Multi-generation family homes with dedicated access
- **The Four Hundred Hall**: Meeting place for descendants of original settlers

#### Midtown Tunnels (Commercial Center)
Busy shopping districts and merchant headquarters serving all creatures.
- **The Great Bazaar**: Indoor market spanning three levels
- **Craftsmouse Quarter**: Traditional trades, apprenticeship guilds
- **Honey Board**: Where Hives products are priced daily
- **Fur & Whisker**: Grooming and social networking center

#### Village Burrows (Bohemian Quarter)
Maze-like informal tunnels housing artists, radicals, and newcomers.
- **The Crumb**: Famous intellectual gathering spot and debate hall
- **Underground Press Alley**: Bark-carved printing blocks, radical publications
- **Cheap Rent Warrens**: Most affordable housing, most "character"
- **The Gnaw**: 24-hour diner for night workers and bohemians

### Notable Locations
- **Grand Central Burrow**: All Underground lines converge here, architectural marvel
- **The Whiskers Building**: Tallest carved structure at 12 stories, mixed use
- **Root Cathedral**: Natural chamber where three oaks meet, used for ceremonies
- **The Squeakeasy**: Hidden bar run by Longtail Family, password required
- **Claw & Associates**: Most prestigious law firm, handles inter-burrow disputes

\columnbreak

## The Branchx - The Canopy Commons

### Districts

#### Old Grove (Traditional Heights)
The original canopy settlement, where height equals status.
- **Branch Level Courts**: Squirrel family compounds at premium heights
- **The High Branch Club**: Exclusive venue for upper canopy families
- **Covered Bridges**: Ancient rope and bark constructions, heavily maintained
- **Emergency Bark Slides**: Rapid evacuation routes installed after hawk attacks

#### New Growth (Working Neighborhoods)
Recently expanded areas housing construction workers and their families.
- **Union Hall**: Nutcracker Union headquarters, center of organizing
- **Tool Libraries**: Communal equipment sharing for construction crews
- **Worker Taverns**: After-shift gathering places with cheap root beer
- **The Failed Tunnel Entrance**: Sealed but still a landmark of broken promises

#### The Tangles (Mixed Housing)
Where different species intermingle in complex rope-and-platform neighborhoods.
- **Courier Central**: Chipmunk racing clubs and dispatch offices
- **Mixed Markets**: Species-diverse shopping with unusual goods
- **Platform Parks**: Public spaces built around major tree junctions
- **Community Centers**: Cross-species gathering places

#### Corvid Corner (Allied Territory)
Where crow allies maintain their embassy and trading posts.
- **The Crow's Nest**: Diplomatic compound off-limits to most mammals
- **Shiny Things Market**: Corvid-run trading post for unusual items
- **Message Towers**: Where crow-carried communications are dispatched
- **The Black Feather**: Tavern where treaties were signed

### Notable Locations
- **Grove Junction Station**: Major Underground stop with famous mosaic murals
- **Bridge 42**: Longest span in the burrow, engineering marvel
- **Nutcracker Arena**: Where construction competitions are held
- **The Splinter**: Notorious tough bar in the lower branches
- **Height Court**: Where branch-level disputes are settled

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

## The Hives - The Crossroads Community

### Districts

#### Central Market (The Great Interchange)
The beating commercial heart where all trade routes converge.
- **The Sorting Yards**: Where goods are distributed to local merchants
- **Three-Line Platform**: Underground junction connecting major routes
- **Wholesale Row**: Bulk goods from external settlements
- **Currency Exchange**: Converting between acorns and barter goods

#### Prairie Dog Quarter (Democratic Hub)
Home to the grassland settlers and their consensus governance.
- **Circle Halls**: Open democratic forums for community decisions
- **The Burrow Network**: Interconnected family tunnels with communal spaces
- **Grassland Goods**: Shops specializing in prairie imports
- **Town Crier Platforms**: Where daily news is announced

#### Rabbit Warrens (Agricultural Nobility)
Traditional farming families with extensive underground complexes.
- **Honey Vaults**: Climate-controlled storage for valuable bee products
- **The Agricultural Exchange**: Seed and harvest futures trading
- **Warren Mansions**: Multi-level family compounds with private gardens
- **Heritage Seed Library**: Preserving traditional varieties

#### Mountain Quarter (Innovation District)
Where guinea pig settlers brought new techniques and perspectives.
- **Terracing Demonstrations**: Showing new agricultural methods
- **The Innovation Hub**: Experimentation with insect partnerships
- **Mountain Crafts Market**: Unique goods from highland traditions
- **Community Kitchens**: Shared cooking spaces with fusion cuisine

### Notable Locations
- **The Great Interchange**: Massive Underground station, three levels
- **Beetle Racing Arena**: Popular entertainment and gambling venue
- **The Honeycomb**: Finest restaurant in the burrow, reservation only
- **Unity Gardens**: Public space celebrating species cooperation
- **The Democratic Archive**: Records of all community decisions

\columnbreak

## Lin's Brook - The Working Waterfront

### Districts

#### Dockside (The Wet Works)
Where water meets commerce in endless activity.
- **Ferry Terminals**: Departures to Scurry Island (when running)
- **Fish Markets**: Dawn auctions of the night's catch
- **Otter Slide Complex**: Competitive racing venue and transit system
- **The Salty Whisker**: Roughest tavern on the waterfront

#### Dam District (Power Center)
The engineering heart providing energy to workshops.
- **The Great Dam**: Marvel of beaver engineering, tours available
- **Power Distribution**: Water wheels driving workshop machinery
- **Engineer's Guild**: Beaver-dominated but accepting apprentices
- **Dam View Overlook**: Tourist spot and romantic meeting place

#### Old Town (Traditional Neighborhood)
Original settlement predating the dam construction.
- **Water Rights Court**: Ancient institution managing stream access
- **Heritage Workshops**: Traditional crafts passed down generations
- **The Current**: Historic tavern where dam plans were drawn
- **Memorial Grove**: Honoring those lost in the Great Flood

#### Greenbank (Gentrification Ground Zero)
Former working-class area transforming rapidly.
- **Artisanal Row**: Craft breweries and specialty goods shops
- **The Conflict Zone**: Where old-timers clash with newcomers
- **Priced Out Memorial**: Graffiti wall documenting displacement
- **The Last Honest Bar**: Holdout against gentrification

### Notable Locations
- **Creek Crossing Station**: Major Underground stop, always damp
- **The Waterworks**: Engineering guild headquarters and museum
- **Silverclaw Compound**: Crime family's "legitimate" businesses
- **The Spillway**: Underground fighting ring location
- **Flood Memorial**: Marking high water from 59 years ago

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

## Scurry Island - The Forgotten Burrow

### Districts

#### The Trunk (Market District)
Built inside the hollow of the fallen giant oak.
- **Black Market Bazaar**: Anything available for the right price
- **The Contraband Corner**: Illegal goods displayed openly
- **Fence Row**: Where stolen goods are "cleaned"
- **No Questions Inn**: Lodging for those needing discretion

#### Root Town (Residential Maze)
Defensive warren of tunnels in the root system.
- **The Disappearing**: Witness protection neighborhood
- **Sanctuary Alley**: Safe houses for creatures on the run
- **The Forgotten**: Where you go to lose your past
- **Underground Underground**: Deeper levels for true anonymity

#### The Crown (Vertical Slums)
Precarious structures built up the dead tree's branches.
- **Desperate Heights**: Cheapest housing, most dangerous
- **Rope Ladder Networks**: Only access to upper levels
- **The Windbreak**: Partial shelter from weather
- **Scavenger's Rest**: Where island's poorest survive

#### Heartwood (The Deep Dark)
Carved into the dead oak's core, mysterious and dangerous.
- **The Archive**: Pre-city artifacts and strange carvings
- **Deep Market**: Truly dangerous goods and services
- **The Quiet Rooms**: Where deals requiring silence are made
- **Ancient Chambers**: Some say pre-Burrow civilization remains

### Notable Locations
- **Ranger Command**: Elite force headquarters facing the Deep Woods
- **Ferry Dock**: Unreliable connection to mainland (usually broken)
- **The Old Giant's Base**: Tourist spot and historical marker
- **Training Grounds**: Where Rangers test recruits
- **The Last Stand**: Memorial to Rangers who didn't return

### Ranger Operations
The Rangers maintain strict protocols for titan defense:
- **Watch Rotations**: Constant surveillance of Deep Woods
- **Quick Response Teams**: Ready to deploy within minutes
- **Evacuation Coordinators**: Working with each burrow's plans
- **Training Academy**: Only the desperate and brave need apply

<div class='note'>

#### <u>Travel Between Burrows</u>

**Underground Transit Times:**
- Mousehattan ↔ Hives: 15 minutes express
- Mousehattan ↔ Branchx: 12 minutes local
- Hives ↔ Lin's Brook: 18 minutes express
- Any ↔ Scurry Island: Ferry only (45 min when running)

**Peak Hours:** Dawn and dusk commutes see severe crowding. Predator alerts can shut down surface routes instantly.

</div>

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

# Careers

## Burrow-Specific Careers

### Acorn Trader *(Mousehattan)*
**Skills:** Charm, Deception, Knowledge (City), Negotiation, Perception, Streetwise, Vigilance, Cool
**Starting Equipment:** Business clothes, ledger, 500 acorns, contact in financial district

### Construction Worker *(The Branchx)*
**Skills:** Athletics, Coordination, Mechanics, Resilience, Survival, Vigilance, Knowledge (Science), Medicine
**Starting Equipment:** Tool kit, safety gear, union membership, work clothes

### Insect Wrangler *(The Hives)*
**Skills:** Animal Handling, Knowledge (Science), Medicine, Perception, Resilience, Survival, Vigilance, Charm
**Starting Equipment:** Whistle, protective gear, insect handling tools, field guide

### Dock Worker *(Lin's Brook)*
**Skills:** Athletics, Coordination, Mechanics, Resilience, Streetwise, Survival, Vigilance, Vehicles
**Starting Equipment:** Work clothes, rope, boat access, union membership

### Ranger *(Scurry Island)*
**Skills:** Athletics, Cool, Perception, Ranged (Light), Survival, Vigilance, Knowledge (Titans), Medicine
**Starting Equipment:** Ranger gear, weapons, emergency supplies, radio

## Cross-Burrow Careers

### Courier
Fast-moving messengers and package delivery specialists who form the communication backbone of the city.

**Skills:** Athletics, Coordination, Perception, Vehicles, Streetwise, Survival, Vigilance, Knowledge (City)
**Starting Equipment:** Delivery bag, route maps, customer contacts, fast transportation

### Crime Family Associate
Connected to the organized crime families that control much of the city's shadow economy.

**Skills:** Coercion, Cool, Deception, Skulduggery, Streetwise, Vigilance, Ranged (Light), Negotiation
**Starting Equipment:** "Family" connections, protection money, concealed weapon

\columnbreak

### Union Organizer
Labor activists working to improve conditions and rights for the city's working creatures.

**Skills:** Charm, Coercion, Leadership, Negotiation, Perception, Streetwise, Knowledge (City), Cool
**Starting Equipment:** Union materials, worker contacts, meeting spaces

### Black Market Dealer
Traders in goods and services that exist outside the legal economy.

**Skills:** Deception, Negotiation, Skulduggery, Streetwise, Vigilance, Knowledge (City), Cool, Perception
**Starting Equipment:** Contraband goods, hidden storage, criminal contacts


<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

# Skills Reference

## Social Skills
- **Charm (Presence):** Persuade to do a favor, appeal to someone's better nature, flirt and seduce, make themselves look good, perform in front of an audience. *Countered by Cool*
- **Coercion (Willpower):** Issue threats, interrogate prisoners, use intimidation. *Countered by Discipline*
- **Deception (Cunning):** Tell lies, mislead people, wear disguises. *Countered by Vigilance*
- **Leadership (Presence):** Rally allies from fear, convince crowds, lead groups. *Countered by Discipline*
- **Negotiation (Presence):** Haggle over purchases, sell goods, broker agreements. *Countered by Negotiation*

## Magic Skills *(Titan-Touched Abilities)*
- **Deer (Intellect):** Stealth, mental manipulation, prediction, luck manipulation
- **Wolf (Cunning):** Pack coordination, enhanced social skills, heightened senses
- **Moose (Willpower):** Resiliency, weather control, telepathy, forest wisdom
- **Bear (Brawn):** Physical augmentation, aggression, increased damage

## Knowledge Skills
- **Knowledge (Science) (Intellect):** Physics, chemistry, biology, engineering, agriculture
- **Knowledge (City) (Intellect):** Physical area and cultural knowledge, politics, the underworld
- **Knowledge (Titans) (Cunning):** Titan behavior, survival tactics, appeasement methods

## Combat Skills
- **Brawl (Brawn):** Fight with bare hands, pin, grapple, hold someone, martial arts
- **Melee (Brawn):** Fight with weapons, duels, armed combat
- **Ranged - Light (Agility):** Smaller hand-held projectile weapons
- **Ranged - Heavy (Agility):** Larger two-handed projectile weapons and emplacements

\columnbreak

## General Skills
- **Animal Handling (Willpower):** Handle non-sapient animals and insects, essential for Hives agriculture
- **Athletics (Brawn):** Climb, swim, jump, run for extended periods
- **Cool (Presence):** Initiative in aware situations, stay calm, gambling, keep nerve
- **Coordination (Agility):** Swing on ropes, walk narrow surfaces, squeeze into spaces, escape restraints
- **Discipline (Willpower):** Confront terror, keep sanity, heal strain, meditate
- **Mechanics (Intellect):** Repair damage, identify parts, design devices, sabotage, build items
- **Medicine (Intellect):** Heal wounds, counteract poison, cure disease, medical procedures
- **Navigation (Intellect):** Read maps, set courses, plot routes under stress
- **Perception (Cunning):** Search for clues, study landscape, conduct surveillance
- **Resilience (Brawn):** Go without sleep, fight off toxins, endure hostile environments
- **Riding (Agility):** Control mounts, mounted combat, calm panicked animals
- **Skulduggery (Cunning):** Pick pockets, pick locks, set traps, study security, distract opponents
- **Stealth (Agility):** Hide, tail someone, infiltrate, move quietly
- **Streetwise (Cunning):** Find black markets, understand slang, approach criminals, navigate cities
- **Survival (Cunning):** Find food and water, notice weather, follow maps, hunt in wilderness
- **Vehicles (Agility):** Operate vehicles safely, dangerous driving, pursue or evade
- **Vigilance (Willpower):** Initiative in ambush situations, catch lies, notice details

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum


# Equipment and Gear

## Species Manufacturing Differences

Different species bring their unique cultural approaches and natural abilities to crafting, resulting in distinct variations of standard equipment.

### Mouse-Made Equipment
- **Modifications:** Add <span class='boost'>b</span> to Mechanics checks when using tools, +1 Accurate quality to ranged weapons
- **Price:** +50% (precision craftsmanship)
- **Aesthetics:** Incredibly detailed and precise construction with intricate engravings

### Rat-Made Equipment
- **Modifications:** Reduce rarity by 1 (mass production), +1 Encumbrance (bulkier but functional)
- **Price:** -25% (efficient manufacturing)
- **Aesthetics:** Practical, robust construction focused on reliability over elegance

### Beaver-Made Equipment
- **Modifications:** +1 Defense (armor), +1 Damage (weapons), +1 Encumbrance (heavier construction)
- **Price:** +25% (superior materials and construction)
- **Aesthetics:** Incredibly sturdy construction built to last generations

### Raccoon-Made Equipment
- **Modifications:** Add Concealable quality, +1 <span class='boost'>b</span> to Skulduggery checks when using tools, rarity +1
- **Price:** +30% (specialized criminal applications)
- **Aesthetics:** Cleverly disguised equipment that appears innocent but serves multiple purposes

### Otter-Made Equipment
- **Modifications:** Waterproof quality, +1 Defense against environmental hazards
- **Price:** +15% (specialized waterproofing)
- **Aesthetics:** Sleek, streamlined design that functions equally well in water and on land. Uses water-resistant materials and sealed construction. Often includes drainage features.

### Rabbit-Made Equipment
- **Modifications:** Add Defensive +1 quality to armor, reduce crafting time by 25%
- **Price:** -10% (community production methods)
- **Aesthetics:** Comfortable, practical design focused on protection and family use. Often includes padding and comfort features. Built for extended wear and community sharing.

### Opossum-Made Equipment
- **Modifications:** Add Stun quality to weapons, equipment appears worthless (Deception bonus)
- **Price:** -50% (appears cheap but functions well)
- **Aesthetics:** Deliberately shabby appearance hiding quality construction. Designed to be underestimated. Often incorporates scavenged materials in clever ways.

### Squirrel-Made Equipment
- **Modifications:** Reduce weight by 1 Encumbrance (minimum 0), add Superior quality to climbing gear
- **Price:** Standard
- **Aesthetics:** Lightweight construction using hollow components and flexible materials. Designed for mobility and storage. Often includes attachment points for securing to trees or rope systems.

### Chipmunk-Made Equipment
- **Modifications:** Add <span class='boost'>b</span> to Athletics checks when using equipment, reduce size by one category
- **Price:** +10% (specialized for speed and agility)
- **Aesthetics:** Compact, streamlined design optimized for rapid movement. Built-in storage pouches and quick-release mechanisms. Everything designed for courier work.

### Mole-Made Equipment
- **Modifications:** Add <span class='boost'>b</span> to underground Navigation, equipment functions in complete darkness
- **Price:** +20% (specialized underground applications)
- **Aesthetics:** Tactile construction with raised surfaces and texture guides. No visual elements needed. Built for underground durability.

### Skunk-Made Equipment
- **Modifications:** Add Intimidating quality, +1 <span class='boost'>b</span> to Coercion when visible
- **Price:** +25% (reputation and specialized construction)
- **Aesthetics:** Bold black and white design that announces the maker. High-quality construction that commands respect. Often includes warning symbols.

### Ferret-Made Equipment
- **Modifications:** Add Flexible quality, can be quickly reconfigured for different uses
- **Price:** +15% (multi-purpose design complexity)
- **Aesthetics:** Modular construction with interchangeable parts. Bright, eye-catching colors and patterns. Built for entertainment and deal-making.

<div class='example'>

##### Using Species Manufacturing
A **Mouse-made Needle Sword** would have Damage 3, Crit 2, Range [Engaged], Encumbrance 1, Price 52 acorns (35 + 50%), *Pierce 1, Accurate 1*

A **Beaver-made Bark Plate** would have Soak +4 (+3 base +1 species), Defense 1, Encumbrance 5 (+1 species), Price 375 acorns (300 + 25%), *Cumbersome 1*

A **Raccoon-made Lockpick Set** would have Price 58 acorns (45 + 30%), *Add <span class='boost'>b</span> to lockpicking, Concealable, Add <span class='boost'>b</span> to Skulduggery checks*

</div>

\columnbreak

## Weapons

### Improvised Weapons
- **Thorn Spear:** Damage 3, Crit 4, Range [Engaged], Encumbrance 2, Price 5 acorns
- **Sling:** Damage 4, Crit 4, Range [Medium], Encumbrance 1, Price 10 acorns
- **Claw Guards:** Damage 2, Crit 3, Range [Engaged], Encumbrance 1, Price 15 acorns, *Defensive 1*
- **Acorn Cap Shield:** Defense +1, Encumbrance 2, Price 8 acorns, *Defensive 1*
- **Sharpened Stick:** Damage 2, Crit 5, Range [Engaged], Encumbrance 1, Price 2 acorns

### Traditional Weapons
- **Nutcracker Club:** Damage 4, Crit 4, Range [Engaged], Encumbrance 3, Price 20 acorns, *Knockdown*
- **Bark Bow:** Damage 5, Crit 3, Range [Long], Encumbrance 2, Price 40 acorns, *Prepare 1*
- **Needle Sword:** Damage 3, Crit 2, Range [Engaged], Encumbrance 1, Price 35 acorns, *Pierce 1*
- **Stone Axe:** Damage 5, Crit 3, Range [Engaged], Encumbrance 3, Price 25 acorns, *Vicious 1*

### Specialized Weapons
- **Beetle Prod:** Damage 2, Crit 5, Range [Engaged], Encumbrance 1, Price 30 acorns, *Stun Damage*
- **Fishing Spear:** Damage 4, Crit 3, Range [Short], Encumbrance 2, Price 18 acorns, *Accurate 1* (underwater)
- **Climbing Pick:** Damage 3, Crit 4, Range [Engaged], Encumbrance 1, Price 22 acorns, *Pierce 1, Defensive 1*

### Ranger Equipment
- **Poison Dart:** Damage 3, Crit 2, Range [Short], Encumbrance 0, Price 25 acorns, *Poison (stun)*
- **Entanglement Net:** Damage 1, Crit 6, Range [Short], Encumbrance 2, Price 50 acorns, *Ensnare 2*
- **Flash Powder:** Damage 0, Crit -, Range [Short], Encumbrance 1, Price 30 acorns, *Blast 3, Stun*
- **Ranger Crossbow:** Damage 6, Crit 3, Range [Long], Encumbrance 3, Price 150 acorns, *Accurate 1, Prepare 1*
- **Smoke Bomb:** Damage 0, Crit -, Range [Short], Encumbrance 1, Price 20 acorns, *Blast 2, Disorient 2*
- **Titan Spear:** Damage 4, Crit 3, Range [Medium], Encumbrance 2, Price 80 acorns, *Pierce 2, Thrown*
- **Emergency Flare:** Damage 1, Crit 5, Range [Long], Encumbrance 1, Price 15 acorns, *Burn 1, Bright light*

### More Specialized Weapons
- **Insect Goad:** Damage 1, Crit 6, Range [Engaged], Encumbrance 1, Price 20 acorns, *Stun Damage, Animal Handling bonus*
- **Rope Dart:** Damage 2, Crit 4, Range [Short], Encumbrance 1, Price 35 acorns, *Ensnare 1, Accurate 1*
- **Bark Shield:** Defense +2, Encumbrance 3, Price 25 acorns, *Defensive 1, Cumbersome 1*
- **Thorn Whip:** Damage 2, Crit 4, Range [Short], Encumbrance 1, Price 30 acorns, *Ensnare 1*
- **Sap Glue Trap:** Damage 0, Crit -, Range [Short], Encumbrance 1, Price 25 acorns, *Immobilize 2*
- **Acorn Sling Staff:** Damage 5, Crit 4, Range [Medium], Encumbrance 2, Price 45 acorns, *Accurate 1, Two-handed*

## Armor

### Light Armor
- **Work Clothes:** Soak +1, Defense 0, Encumbrance 1, Price 20 acorns
- **Leather Vest:** Soak +1, Defense 1, Encumbrance 1, Price 45 acorns
- **Padded Jacket:** Soak +2, Defense 0, Encumbrance 2, Price 75 acorns
- **Courier Gear:** Soak +1, Defense 1, Encumbrance 1, Price 60 acorns, *Reduces falling damage by 1*

### Medium Armor
- **Scale Mail:** Soak +2, Defense 1, Encumbrance 2, Price 120 acorns, *Made from overlapping bark scales*
- **Reinforced Vest:** Soak +3, Defense 0, Encumbrance 3, Price 150 acorns
- **Guild Armor:** Soak +2, Defense 1, Encumbrance 2, Price 180 acorns, *Includes tool attachments*

### Heavy Armor
- **Ranger Gear:** Soak +2, Defense 1, Encumbrance 3, Price 200 acorns, *Environmental protection*
- **Bark Plate:** Soak +3, Defense 1, Encumbrance 4, Price 300 acorns, *Cumbersome 1*
- **Shell Armor:** Soak +4, Defense 0, Encumbrance 5, Price 450 acorns, *Cumbersome 2, made from large insect shells*

### Specialized Armor
- **Diving Suit:** Soak +1, Defense 0, Encumbrance 2, Price 100 acorns, *Waterproof, allows underwater breathing*
- **Climbing Harness:** Soak +1, Defense 1, Encumbrance 1, Price 80 acorns, *Prevents falling damage up to Medium range*
- **Winter Coat:** Soak +2, Defense 0, Encumbrance 2, Price 90 acorns, *Cold weather protection*

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum


# Arts and Entertainment

The Great Burrow's cultural life reflects diverse species and unique urban forest challenges.

## Theater and Performance

### The Grand Oak Theater *(Mousehattan)*
- **Location:** Carved into the base of the Trading Oak
- **Capacity:** 800 creatures across four tiers
- **Programming:** Classical dramas, modern comedies, musical revues
- **Audience:** Primarily upper-class mice and rats
- **Notable Productions:** "The Merchant of Mousehattan," "A Midsummer Night's Squeak"

### The People's Stage *(The Branchx)*
- **Location:** Natural amphitheater formed by intersecting branches
- **Capacity:** 1,200 creatures, standing room only
- **Programming:** Union rallies, folk performances, political satire
- **Audience:** Working-class creatures from all burrows
- **Notable Productions:** "The Nutcracker's Revenge," "Bridges of Madison County (Tree)"

### The Crossroads Theater *(The Hives)*
- **Location:** Multiple venues throughout the burrow, rotating between districts
- **Programming:** Immigrant stories, fusion works, cultural celebrations
- **Audience:** Most diverse in the city, heavy working-class and immigrant attendance
- **Cultural Impact:** Showcases immigrant experiences and promotes cultural understanding

\columnbreak

## Visual Arts

### The Mousehattan Museum of Natural Arts
- **Collection:** Ancient acorns, preserved leaves, mineral specimens, fossils
- **Special Exhibitions:** Rotating displays of contemporary creature art
- **Education Programs:** Art classes for young creatures
- **Controversy:** Debates over "modern" vs. "traditional" art

### The Canopy Gallery Circuit *(The Branchx)*
- **Format:** Art displayed on bridge supports and tree trunks
- **Artists:** Working creatures creating in spare time
- **Themes:** Labor, community, resistance to gentrification
- **Medium:** Bark carvings, rope sculptures, found object installations

### The Hives Cultural Collective
- **Focus:** Multicultural art celebrating immigrant traditions and fusion
- **Products:** Prairie dog pottery, marmot stonework, guinea pig textiles
- **Philosophy:** Art as bridge between cultures, celebrating diversity
- **Innovation:** Cross-cultural artistic techniques creating new art forms

<div class='note'>

#### <u>Cultural Venues by Burrow</u>

**Mousehattan:** Grand Oak Theater, Museum of Natural Arts, exclusive private galleries

**The Branchx:** People's Stage, Canopy Gallery Circuit, union-sponsored murals

**The Hives:** Crossroads Theater, Cultural Collective, rotating cultural festivals

**Lin's Brook:** Waterfront performance spaces, folk music traditions, craftsman workshops

**Scurry Island:** Death Theater, underground galleries, survival-themed performances

</div>

<div class=\"footnote\">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

## Communication Systems

### Newspapers
- **The Daily Squeak:** City-wide circulation, conservative editorial policy, covers financial markets and politics (Mousehattan-based)
- **The Workers' Voice:** Pro-labor newspaper serving The Branchx and Lin's Brook, union news and worker rights
- **Hives Harmony:** Community newsletter covering farming tips, cultural exchange, and cooperative values
- **The Island Gazette:** Scurry Island publication with survival tips, Ranger news, and black market information

### Messaging Services
- **Chipmunk Courier Network:** City-wide package delivery and message service, same-day delivery within city
- **Bat Night Service:** Specialized after-hours and emergency communications, fastest available service
- **Underground Mail:** Secure tunnel-based communications, weather-independent and confidential
- **Crow Network:** Information brokerage with corvids, payment in shiny objects or favors

\columnbreak

### Public Information Systems
- **Town Criers:** Frogs and toads making public announcements at major gathering places
- **Bulletin Boards:** Community job postings, housing notices, and event information
- **Signal Systems:** Smoke signals, bell networks, flag systems, drum networks, firefly light signals

<div class='example'>

##### Communication in Daily Life
A typical creature might start the day reading The Daily Squeak over breakfast, send a message via chipmunk courier for work, check the community bulletin board for evening events, and hear the evening town crier announce weather warnings for tomorrow.

</div>

## Festivals and Celebrations

### The Great Burrow Calendar
**Seasonal Structure:** Spring Awakening (renewal, planting), Summer Growth (peak activity, construction), Autumn Harvest (gathering, gratitude), Winter Rest (reflection, community bonding)

### Major Festivals

#### The Great Awakening *(Spring Equinox)*
City-wide celebration of renewal and new beginnings. Communities plant new gardens, begin construction projects, and hold renewal ceremonies.

#### Midsummer Construction Festival
Celebrating the peak building season. Competitions between construction crews, displays of craftsmanship, and community barn-raising events.

#### Harvest Gratitude *(Autumn Equinox)*
Thanksgiving for the year's abundance. Each burrow contributes traditional foods, cultural performances showcase diversity, and communities share resources for winter preparation.

#### The Long Night *(Winter Solstice)*
Community bonding during the darkest time. Underground gatherings with storytelling, planning for next year, and mutual aid distribution.

<div class=\"footnote\">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

## Insect-Powered Technology

### Communication
- **Messenger Beetle (Basic):** 80% delivery success, Range: City-wide, Price 30 acorns
- **Messenger Beetle (Premium):** 95% delivery success, Range: Regional, Price 85 acorns
- **Butterfly Messenger:** Delicate but fast communication, Price 35 acorns, *90% success, same-day delivery within city*

### Professional Tools
- **Insect Whistle:** Animal Handling tool for managing insects, Price 30 acorns, *Add <span class='boost'>b</span> to insect-related checks*
- **Beetle Cart:** Small cargo transport, Price 200 acorns, *Carries 5 Encumbrance, requires trained beetle*
- **Ant Farm Calculator:** Living computation device, Price 150 acorns, *Add <span class='boost'>b</span><span class='boost'>b</span> to complex mathematical calculations*

### Advanced Systems
- **Spider Silk Rope:** Ultra-strong climbing rope, Price 60 acorns, *Half normal Encumbrance, Superior quality*
- **Cricket Alarm:** Security system using trained crickets, Price 80 acorns, *Alerts to intruders within Short range*
- **Silk Parachute:** Emergency descent device, Price 100 acorns, *Prevents falling damage from any height*

### Tools and Equipment

#### Communication
- **Messenger Beetle (Basic):** 80% delivery success, Range: City-wide, Price 30 acorns, *Must be familiar with recipient*
- **Messenger Beetle (Premium):** 95% delivery success, Range: Regional, Price 85 acorns, *Must be familiar with recipient*
- **Signal Mirror:** Reflects light for long-distance communication, Price 12 acorns
- **Message Tube:** Waterproof container for important documents, Price 6 acorns

#### Professional Tools
- **Tunnel Digging Kit:** Mechanics tools for underground work, Price 150 acorns, *Add <span class='boost'>b</span> to underground construction*
- **Insect Whistle:** Animal Handling tool for managing insects, Price 30 acorns, *Add <span class='boost'>b</span> to insect-related checks*
- **Climbing Gear:** Athletics equipment for canopy travel, Price 100 acorns, *Add <span class='boost'>b</span> to climbing checks*
- **Lockpick Set:** Skulduggery tools for opening locks, Price 45 acorns, *Add <span class='boost'>b</span> to lockpicking*
- **Medical Kit:** Medicine supplies for treating injuries, Price 80 acorns, *Add <span class='boost'>b</span> to Medicine checks*
- **Carpenter's Tools:** Mechanics tools for woodworking, Price 60 acorns, *Add <span class='boost'>b</span> to construction checks*

#### Survival Gear
- **Emergency Rations:** 3 days food, Price 15 acorns
- **Water Purification Tablets:** Makes questionable water safe, Price 10 acorns (10 uses)
- **Rope (50 feet):** Strong woven fiber rope, Price 20 acorns, Encumbrance 2
- **Grappling Hook:** For climbing and swinging, Price 35 acorns, Encumbrance 1
- **Sleeping Bag:** Warm bedding for outdoor rest, Price 25 acorns, Encumbrance 2
- **Fire Starting Kit:** Flint, tinder, and kindling, Price 8 acorns

#### Lighting
- **Firefly Lantern:** Light source (living), Price 40 acorns, requires daily feeding, *Bright light, Medium range*
- **Candle:** Simple wax light source, Price 2 acorns, *Dim light, Short range, 4 hour duration*
- **Torch:** Burning stick for light, Price 1 acorn, *Bright light, Short range, 1 hour duration*
- **Glowworm Jar:** Portable dim light, Price 15 acorns, *Dim light, Short range, no fuel needed*

#### Specialized Equipment
- **Magnifying Glass:** For detailed work, Price 50 acorns, *Add <span class='boost'>b</span> to Perception checks for small details*
- **Scales:** For precise measurements, Price 30 acorns, *Required for accurate trading*
- **Compass:** Navigation aid, Price 40 acorns, *Add <span class='boost'>b</span> to Navigation checks*
- **Spyglass:** For distant observation, Price 120 acorns, *See clearly at Long range*
- **Weather Vane:** Predicts weather changes, Price 25 acorns, *Add <span class='boost'>b</span> to weather prediction*

#### Insect-Powered Technology
- **Beetle Cart:** Small cargo transport, Price 200 acorns, *Carries 5 Encumbrance, requires trained beetle*
- **Ant Farm Calculator:** Living computation device, Price 150 acorns, *Add <span class='boost'>b</span><span class='boost'>b</span> to complex mathematical calculations*
- **Spider Silk Rope:** Ultra-strong climbing rope, Price 60 acorns, *Half normal Encumbrance, Superior quality*
- **Honeycomb Storage:** Organized storage system, Price 40 acorns, *Reduces effective Encumbrance of stored items by 1*
- **Cricket Alarm:** Security system using trained crickets, Price 80 acorns, *Alerts to intruders within Short range*
- **Butterfly Messenger:** Delicate but fast communication, Price 35 acorns, *90% success, same-day delivery within city*
- **Beetle Mill:** Portable grinding device, Price 120 acorns, *Processes grain and nuts, requires beetle labor*
- **Silk Parachute:** Emergency descent device, Price 100 acorns, *Prevents falling damage from any height*

## Transportation

### Personal Transport
- **Acorn Cap Boat:** Single creature, water travel, Price 100 acorns
- **Bark Sled:** Ground transport, can carry cargo, Price 50 acorns
- **Rope Harness:** For climbing/swinging, Price 25 acorns

### Public Transport
- **Underground Pass:** Monthly unlimited subway travel, Price 20 acorns
- **Ferry Ticket:** Single crossing to Scurry Island, Price 2 acorns
- **Courier Service:** Message delivery, Price 1-5 acorns depending on distance


<div class='note'>

#### <u>Currency: The Acorn Standard</u>

The Great Burrow operates on the Acorn Standard, with currency valued by the quality and preparation of acorns:

- **Fresh Acorns:** Basic currency, 1-2 acorn value
- **Aged Acorns:** Higher value, 3-5 acorn value  
- **Prepared Acorns:** Processed and preserved, 5-10 acorn value
- **Prime Acorns:** Perfect specimens, 10+ acorn value

Trade also happens through barter, especially for specialized services and rare goods.

</div>


\columnbreak
<div class='example'>


##### Equipment in Action
Vera the chipmunk courier is upgrading her gear. She purchases a **Squirrel-made** rope harness for climbing, which reduces the weight by 1 Encumbrance (minimum 0) and adds Superior quality for climbing applications. 

She also invests in a **Premium Messenger Beetle** for important deliveries, giving her a reliable 95% success rate for regional communications - essential for her growing business reputation.

</div>

<div class='note'>

#### <u>Seasonal Equipment Needs</u>

Equipment needs change dramatically with the seasons in The Great Burrow:

**Winter:** Heating systems, preserved food, ice-travel gear
**Spring:** Flood protection, construction materials, planting supplies  
**Summer:** Cooling systems, water storage, fire prevention
**Autumn:** Harvest tools, storage systems, preservation equipment

</div>

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

# New Talents

## Tier 1 Talents

### Burrow Native *(Passive)*
Choose one burrow. Remove <span class='setback'>b</span> from all social and navigation checks in that burrow. Add <span class='boost'>b</span> to Streetwise checks related to that burrow's culture and politics.

### Species Solidarity *(Passive)*
Add <span class='boost'>b</span> to social checks when interacting with creatures of the same species. This bonus increases to <span class='boost'>b</span><span class='boost'>b</span> when dealing with family or clan members.

### Tunnel Fighter *(Passive)*
When fighting in confined spaces (tunnels, burrows, etc.), add <span class='boost'>b</span> to combat checks and increase defense by 1.

### Predator Awareness *(Passive)*
Add <span class='boost'>b</span> to Vigilance checks to detect aerial predators. When a predator is spotted, may spend 1 strain to immediately move to cover as an out-of-turn incidental.

### Union Member *(Passive)*
Gain access to union resources, legal aid, and worker solidarity. Add <span class='boost'>b</span> to social checks with other union members. Reduce cost of certain services by 25%.

## Tier 2 Talents

### Crime Family Connected *(Passive)*
Gain protection and resources from organized crime, but also obligations. Add <span class='boost'>b</span><span class='boost'>b</span> to Streetwise checks in criminal contexts. Reduce difficulty of acquiring illegal goods by 1.

### Titan Survivor *(Passive)*
Having survived a direct titan encounter, add <span class='boost'>b</span> to all checks related to giant creatures. Other creatures treat you with respect/fear. Once per session, may add <span class='boost'>b</span><span class='boost'>b</span> to a Cool or Discipline check.

### Master Craftscreature *(Passive)*
Choose one type of crafting (construction, insect management, etc.). Add <span class='boost'>b</span><span class='boost'>b</span> to all related checks. Reduce time and cost of creating items by 25%.

\pagebreakNum

## Tier 3 Talents

### Burrow Boss *(Passive)*
Leadership position in burrow hierarchy. Add <span class='boost'>b</span><span class='boost'>b</span> to Leadership checks. Can call upon significant resources and followers. Gain political influence but also enemies.

### Ranger Elite *(Passive)*
Veteran of multiple titan encounters. Add <span class='boost'>b</span><span class='boost'>b</span> to all combat checks against large creatures. Gain access to advanced Ranger equipment and tactics.

### Underground Railroad *(Active)*
Can help creatures disappear from their old lives and start new ones. Once per session, can provide false identity, safe passage, or sanctuary for any creature.

### Titan Affinity *(Passive)*
*Prerequisite: Survived an encounter with a Titan, or DM approval*
One of the Titan-related skills becomes a career skill for you, based on the titan you have encountered.

## Tier 4 Talents

### Burrow Legend *(Passive)*
Your reputation precedes you throughout the city. Add <span class='boost'>b</span><span class='boost'>b</span> to all social checks within your home burrow. Once per session, may call upon your reputation to gain a significant favor or resource.

### Titan Whisperer *(Active)*
Your connection to the giants runs deeper than most. Once per session, may attempt to communicate with or influence a titan's behavior. This requires a Formidable (<span class='difficulty'>d</span><span class='difficulty'>d</span><span class='difficulty'>d</span><span class='difficulty'>d</span><span class='difficulty'>d</span>) Knowledge (Titans) check.

### Master of Networks *(Passive)*
Your web of contacts spans the entire city. Start each session with 3 "favor tokens" that can be spent to gain information, resources, or assistance from contacts throughout The Great Burrow.

\pagebreakNum

## Species-Specific Talents

### Mouse Precision *(Passive)*
*Prerequisite: Mouse species*

Your natural attention to detail serves you well. When making Mechanics or Medicine checks, may spend 2 strain to upgrade the ability of the check twice instead of once.

### Rat Networking *(Passive)*
*Prerequisite: Rat species*

Your species' natural entrepreneurial spirit opens doors. Reduce the difficulty of Streetwise and Negotiation checks by 1 when dealing with business matters.

### Squirrel Storage *(Passive)*
*Prerequisite: Squirrel species*

Your hoarding instincts are legendary. Increase your Encumbrance Threshold by 3. Once per session, may produce a useful common item that you "had stored away."

### Beaver Engineering *(Passive)*
*Prerequisite: Beaver species*

Your construction expertise is unmatched. When making Mechanics checks related to building or repair, add <span class='boost'>b</span><span class='boost'>b</span> to the check and reduce the time required by half.

### Otter Flow *(Passive)*
*Prerequisite: Otter species*

Your natural grace in water extends to all movement. Add <span class='boost'>b</span> to all Athletics and Coordination checks. When in water, upgrade the ability of these checks once.

### Rabbit Warren Leader *(Passive)*
*Prerequisite: Rabbit species*

Your community instincts make you a natural organizer. When leading a group of 3 or more creatures, all group members gain <span class='boost'>b</span> to checks that benefit from coordination. You may use Leadership instead of other social skills when dealing with family or community matters.

### Guinea Pig Innovation *(Active)*
*Prerequisite: Guinea pig species*

Your mountain heritage brings fresh perspectives to old problems. Once per session, when facing a challenge that has stumped others, you may spend 2 strain to propose an unconventional solution that adds <span class='boost'>b</span><span class='boost'>b</span> to the attempt and reduces the difficulty by 1.

### Opossum Survivor *(Passive)*
*Prerequisite: Opossum species*

Your species' reputation for resilience is well-earned. When reduced to 0 wounds, you may immediately use your "Play Dead" ability as an out-of-turn incidental. Additionally, add <span class='boost'>b</span> to all checks made while appearing dead or unconscious.

### Raccoon Fence Master *(Passive)*
*Prerequisite: Raccoon species*

Your natural dexterity and criminal connections serve you well. Reduce the difficulty of acquiring illegal goods by 1. When "washing" stolen goods, add <span class='boost'>b</span><span class='boost'>b</span> to Deception checks to make them appear legitimate.

### Chipmunk Speed Burst *(Active)*
*Prerequisite: Chipmunk species*

Your legendary speed can be pushed to extraordinary limits. Once per encounter, may move to any location within Long range as a maneuver. Suffer 4 strain after using this ability.

### Mole Tunnel Sense *(Passive)*
*Prerequisite: Mole species*

Your vibration sense extends beyond mere detection. You can "read" the structural integrity of underground spaces, predict cave-ins, and find hidden passages. Add <span class='boost'>b</span><span class='boost'>b</span> to Navigation checks underground and <span class='boost'>b</span> to Perception checks to detect structural weaknesses.

### Skunk Reputation *(Passive)*
*Prerequisite: Skunk species*

Your natural deterrent has made you a master of intimidation without violence. Upgrade Coercion checks once when the threat of your chemical defense is relevant. Enemies must make an Average (<span class='difficulty'>d</span><span class='difficulty'>d</span>) Discipline check to attack you in melee range under similar circumstances.

### Badger Territory *(Passive)*
*Prerequisite: Badger species*

Your territorial instincts extend to any space you claim as your own. When defending any location you've spent at least 24 hours in, add <span class='boost'>b</span><span class='boost'>b</span> to all combat checks and increase your Defense by 1. Other creatures instinctively respect your claimed territory.

### Ferret Deal Maker *(Active)*
*Prerequisite: Ferret species*

Your hyperactive nature and flexible morality make you an excellent negotiator. Once per session, when making a Negotiation check, you may spend 2 strain to add <span class='boost'>b</span><span class='boost'>b</span> to the check and allow both parties to gain something they want, even from seemingly impossible situations.

### Weasel Information Network *(Passive)*
*Prerequisite: Weasel species*

Your species' reputation for knowing everything serves you well. Start each session with one piece of useful information about the current situation. Additionally, reduce the difficulty of Streetwise checks to gather information by 1.

### Bat Night Vision *(Passive)*
*Prerequisite: Bat species*

Your echolocation and flight give you unparalleled awareness. You can "see" in complete darkness and through light cover. Add <span class='boost'>b</span> to all Perception checks and <span class='boost'>b</span><span class='boost'>b</span> to Vigilance checks made during night hours or in darkness.

### Shrew Insect Bond *(Active)*
*Prerequisite: Shrew species*

Your ultrasonic communication has created a deep bond with a specific insect companion. Choose one insect type (beetle, ant, cricket, etc.). You have a loyal insect companion that can perform simple tasks, deliver messages, and provide assistance. The insect has 3 wounds, 2 strain, and relevant skills at 2 dice. If it dies, you can bond with a new one after 1 week.

## Insect Companion Talents

### Wasp Guardian *(Active)*
*Prerequisite: Animal Handling 2, must have befriended a wasp*

You have formed a bond with a loyal wasp companion. The wasp has 4 wounds, 3 strain, and will defend you fiercely. Once per encounter, the wasp can make a sting attack (Damage 3, Crit 3, Poison) against enemies within Short range. If the wasp is killed, you suffer 2 strain and cannot bond with another for 2 weeks.

### Beetle Mount *(Passive)*
*Prerequisite: Animal Handling 3, Riding 2*

You have trained a large beetle as a mount. The beetle can carry you and moderate cargo, has 8 wounds, 4 strain, and moves at your speed. It can also assist with heavy labor, adding <span class='boost'>b</span> to Mechanics checks involving construction or hauling. Requires daily feeding and care.

### Cricket Alarm *(Passive)*
*Prerequisite: Animal Handling 2*

You have bonded with a cricket that serves as an early warning system. The cricket alerts you to danger within Medium range, adding <span class='boost'>b</span><span class='boost'>b</span> to Initiative checks and Vigilance checks to avoid surprise. The cricket can also relay simple messages through its chirping patterns.

### Ant Colony Contact *(Active)*
*Prerequisite: Animal Handling 3, must have Shrew Insect Bond or similar*

You have established communication with a local ant colony. Once per session, you can request the colony's assistance for information gathering, small item transport, or creating diversions. The ants will perform reasonable tasks that don't endanger the colony.

\pagebreakNum

# Magic and Unexplained Phenomena

## Setting Magic Level: Very Low

The Great Burrow is fundamentally a **low-magic setting** where unexplained phenomena are rare, poorly understood, and often dismissed as folklore by the general population. What might be called "magic" in other settings manifests here as subtle abilities tied to traumatic or profound encounters with the titans that walk the forest.

### The Nature of "Magic"

#### No Traditional Magic
- No wizards, spells, or magical items in the conventional sense
- No magical creatures (beyond the titans themselves)
- No supernatural forces that creatures can reliably study or harness
- Most citizens live their entire lives without witnessing anything truly unexplainable

#### Titan-Touched Phenomena
What passes for magic comes from direct encounters with the giants:
- **Deer Blessings:** Survivors of deer encounters sometimes develop uncanny luck or intuition
- **Bear Marks:** Those who survive bear attacks may gain primal strength or fearsome presence
- **Wolf Touched:** Extremely rare, grants predatory instincts and pack awareness
- **Moose Blessed:** Rarest of all, survivors report connection to forest rhythms and weather

### Mechanical Implementation

#### Titan-Touched Talents

**Tier 1: Awakening**
- **Blessed Instincts** *(Passive)*: Once per session, may upgrade the ability of any skill check before rolling
- **Titan's Mark** *(Passive)*: Other creatures can sense something different about you. Add <span class='boost'>b</span> to Coercion checks, but add <span class='setback'>b</span> to some social interactions
- **Uncanny Luck** *(Active)*: Spend 1 strain to reroll any dice pool, but must accept the second result

**Tier 2: Manifestation**
- **Forest Whispers** *(Active)*: Once per session, gain insight about immediate area or recent events (GM provides one useful piece of information)
- **Primal Presence** *(Passive)*: When dealing with non-sapient animals, may use Coercion or Charm without penalty
- **Survivor's Edge** *(Passive)*: When reduced to half wounds or strain, gain <span class='boost'>b</span> to all checks until fully healed

**Tier 3: Integration**
- **Titan's Shadow** *(Active)*: Once per session, may add <span class='boost'>b</span><span class='boost'>b</span><span class='boost'>b</span> to any check related to survival, combat, or protecting others
- **Deep Knowing** *(Active)*: Spend 2 strain and a story point to ask the GM one question about the current situation and receive a truthful answer
- **Pack Leader** *(Passive)*: Allies within Short range gain <span class='boost'>b</span> to checks when you spend strain to assist them

#### Acquiring Titan-Touched Status
- **Direct Titan Encounter:** Survive a face-to-face meeting with a giant creature
- **Profound Trauma:** Experience something that fundamentally changes your worldview
- **Spiritual Awakening:** Deep meditation or religious experience in sacred locations
- **Inherited Sensitivity:** Very rare, passed down through bloodlines (1 in 1000 creatures)

#### Social Implications
- **Urban Skepticism:** Most city dwellers dismiss titan-touched abilities as coincidence or delusion
- **Ranger Respect:** Rangers recognize and value these abilities, even if they don't understand them
- **Religious Significance:** Titan Speakers often display these phenomena, reinforcing their spiritual authority
- **Scientific Denial:** Academics and intellectuals actively debunk claims of supernatural abilities

### Power Manifestations by Titan Type

#### Deer-Blessed *(The Fortunate)*
- Abilities manifest as incredible timing and serendipitous events
- Enhanced intuition about people's true intentions
- Uncanny ability to find exactly what they need when they need it
- Sometimes experience prophetic dreams or visions

**Sample Powers:**
- **Serendipity:** Beneficial coincidences occur more frequently
- **True Sight:** Can sense when others are lying or hiding something
- **Path Finding:** Always know the best route to take, even in unfamiliar territory

#### Bear-Marked *(The Fierce)*
- Abilities manifest as enhanced physical presence and primal instincts
- Intimidating aura that affects both creatures and animals
- Enhanced strength and endurance during crisis situations
- Natural leadership in dangerous situations

**Sample Powers:**
- **Primal Roar:** Voice can carry incredible distances and inspire fear
- **Iron Will:** Resistance to fear, intimidation, and mental influence
- **Protective Fury:** Enhanced combat abilities when defending others

#### Wolf-Touched *(The Hunters)*
- Extremely rare due to limited wolf contact in the region
- Enhanced pack instincts and ability to coordinate with others
- Predatory awareness and tracking abilities
- Instinctive understanding of hierarchy and dominance

**Sample Powers:**
- **Pack Sense:** Awareness of allies' conditions and intentions
- **Hunter's Instinct:** Enhanced tracking and pursuit abilities
- **Alpha Presence:** Natural leadership and ability to command respect

#### Moose-Blessed *(The Wise)*
- Rarest manifestation, tied to deep forest wisdom
- Connection to seasonal cycles and weather patterns
- Enhanced understanding of natural systems and ecology
- Ability to sense disturbances in the forest's balance

**Sample Powers:**
- **Weather Sense:** Predict weather changes and natural disasters
- **Forest Speech:** Limited communication with non-sapient forest creatures
- **Seasonal Wisdom:** Enhanced knowledge of natural cycles and timing

### Using Magic in Campaigns

#### Rarity Guidelines
- **1 in 100 creatures** might have some minor sensitivity
- **1 in 1000 creatures** have noticeable abilities
- **1 in 10,000 creatures** have significant powers
- **Player characters** are exceptional and may have higher rates

#### Discovery and Development
- Abilities often manifest during stress or crisis
- Development is instinctive, not learned
- No teachers or schools exist for these phenomena
- Powers may fade if not used or may grow stronger with experience

#### Campaign Integration
- **Urban Fantasy:** Focus on how abilities affect daily life in the city
- **Mystery:** Investigate unexplained phenomena and their sources
- **Social Drama:** Deal with skepticism, fear, or exploitation of abilities
- **Environmental:** Use powers to protect the forest and its creatures

#### GM Guidelines
- **Keep it Subtle:** Powers should enhance rather than dominate gameplay
- **Maintain Mystery:** Never fully explain how or why abilities work
- **Social Consequences:** Consider how others react to unexplained phenomena
- **Narrative Focus:** Use powers to drive story rather than solve problems easily

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

# Environmental Rules

## Titan Encounters

When titans (bears, deer, moose, etc.) appear, use these special rules:

### Titan Combat
- **Titans are Silhouette 4-6** depending on species
- **Cannot be directly fought** by player characters under normal circumstances
- **Focus on escape, distraction, or environmental solutions**
- **Titan attacks cause massive area damage**
- **Success means survival and escape, not victory**

<div class='example'>

##### Titan Encounter
The characters are in Mousehattan when the warning bells ring - a deer has been spotted approaching the Trading Oak. Rather than fighting the massive creature, they must:

- Help evacuate civilians to deep shelters
- Protect important documents from the Acorn Exchange
- Create diversions using offering piles
- Navigate through panicking crowds
- Avoid being stepped on during the chaos

Success is measured by how many lives they save and how much of the city's infrastructure survives, not by defeating the titan.

</div>

## Predator Encounters

### Aerial Predators (Hawks, Owls)
- **Surprise Attacks:** Predators get <span class='boost'>b</span><span class='boost'>b</span> on initial attack if creatures are in open
- **Cover is Essential:** Being under cover provides complete protection
- **Group Tactics:** Predators focus on isolated creatures
- **Escape Options:** Reaching cover, underground access, or group defense

### Ground Predators (Snakes, Foxes)
- **Stealth Hunters:** Use Stealth vs. Vigilance for surprise
- **Terrain Advantage:** Predators know local hunting grounds
- **Seasonal Patterns:** Some predators only active certain times
- **Warning Systems:** Community alerts can provide advance notice

\columnbreak

## Weather and Seasonal Effects

### Spring
- **Flooding:** Athletics checks to navigate, some areas inaccessible
- **Mating Season:** Increased territorial disputes, social complications
- **Construction Season:** More work available, increased activity

### Summer
- **Heat Waves:** Resilience checks for extended outdoor activity
- **Drought:** Water becomes precious, affects Lin's Brook economy
- **Peak Activity:** All systems running at maximum capacity

### Autumn
- **Harvest Season:** Economic boom, but also increased competition
- **Storm Season:** Piloting checks for travel, infrastructure damage
- **Preparation Pressure:** Social stress as creatures prepare for winter

### Winter
- **Cold:** Survival checks without proper shelter/clothing
- **Food Scarcity:** Increased prices, social tensions
- **Limited Travel:** Some routes become impassable

<div class='note'>

#### <u>Seasonal Adventures</u>

Each season brings different challenges and opportunities:

**Spring:** Flood rescue, construction projects, mating season drama
**Summer:** Titan encounters, drought management, peak trading
**Autumn:** Harvest competitions, storm preparations, hoarding conflicts  
**Winter:** Survival challenges, political intrigue, resource sharing

</div>

## Environmental Hazard Tables

### Titan Encounter Table (d100)
  - **01-40:** None — Normal operations
  - **41-60:** Deer (Moderate) — Evacuate upper levels
  - **61-75:** Wild Boar (High) — Tunnel collapse risk
  - **76-85:** Bear (Extreme) — Full evacuation
  - **86-95:** Multiple (Critical) — City-wide emergency
  - **96-00:** Moose (Catastrophic) — Abandon district

### Predator Activity by Time (d100)

- **01-30:** Dawn: Hawks — Day: Clear — Dusk: Hawks — Night: Owls
- **31-50:** Dawn: Foxes — Day: Hawks — Dusk: Foxes — Night: Snakes
- **51-70:** Dawn: Clear — Day: Clear — Dusk: Snakes — Night: Foxes
- **71-85:** Dawn: Multiple — Day: Corvids — Dusk: Multiple — Night: Multiple
- **86-00:** Dawn: Surprise — Day: Clear — Dusk: Surprise — Night: Surprise

### Weather Severity Table

- **Spring:** Minor (<span class='difficulty'>d</span>): Light rain — Moderate (<span class='difficulty'>d</span><span class='difficulty'>d</span>): Flooding risk — Severe (<span class='difficulty'>d</span><span class='difficulty'>d</span><span class='difficulty'>d</span>): Flash floods
- **Summer:** Minor (<span class='difficulty'>d</span>): Hot day — Moderate (<span class='difficulty'>d</span><span class='difficulty'>d</span>): Heat wave — Severe (<span class='difficulty'>d</span><span class='difficulty'>d</span><span class='difficulty'>d</span>): Drought
- **Autumn:** Minor (<span class='difficulty'>d</span>): Wind — Moderate (<span class='difficulty'>d</span><span class='difficulty'>d</span>): Storm — Severe (<span class='difficulty'>d</span><span class='difficulty'>d</span><span class='difficulty'>d</span>): Hurricane
- **Winter:** Minor (<span class='difficulty'>d</span>): Cold snap — Moderate (<span class='difficulty'>d</span><span class='difficulty'>d</span>): Snow — Severe (<span class='difficulty'>d</span><span class='difficulty'>d</span><span class='difficulty'>d</span>): Blizzard

### Environmental Difficulty Modifiers
- **Heavy Rain:** Add <span class='setback'>b</span> to physical activities
- **Flooding:** Upgrade difficulty once for movement
- **High Wind:** Add <span class='setback'>b</span><span class='setback'>b</span> to ranged attacks
- **Snow/Ice:** Add <span class='setback'>b</span> to Athletics, upgrade once for climbing
- **Extreme Heat:** Resilience check or suffer 2 strain per hour
- **Darkness:** Add <span class='setback'>b</span><span class='setback'>b</span> to Perception and combat

\columnbreak

### Titan Warning Times

- **Ranger Scouts:** 30 minutes warning — Evacuation Difficulty: <span class='ability'>d</span><span class='ability'>d</span>
- **Crow Allies:** 20 minutes warning — Evacuation Difficulty: <span class='difficulty'>d</span><span class='difficulty'>d</span>
- **Ground Tremors:** 10 minutes warning — Evacuation Difficulty: <span class='difficulty'>d</span><span class='difficulty'>d</span><span class='difficulty'>d</span>
- **Visual Sighting:** 5 minutes warning — Evacuation Difficulty: <span class='challenge'>c</span><span class='difficulty'>d</span><span class='difficulty'>d</span>
- **No Warning:** 0 minutes warning — Evacuation Difficulty: <span class='challenge'>c</span><span class='challenge'>c</span><span class='difficulty'>d</span>

### Predator Escape Options

- **Open Ground:** Sprint to cover — Athletics (<span class='difficulty'>d</span><span class='difficulty'>d</span><span class='difficulty'>d</span>)
- **Near Trees:** Climb to safety — Athletics (<span class='difficulty'>d</span><span class='difficulty'>d</span>)
- **Near Water:** Dive and swim — Athletics (<span class='difficulty'>d</span><span class='difficulty'>d</span>)
- **In Group:** Defensive circle — Cool (<span class='difficulty'>d</span>) + numbers
- **Underground:** Duck into tunnel — Perception (<span class='difficulty'>d</span><span class='difficulty'>d</span>) to find

### Infrastructure Damage

- **Titan Step:** Tunnel collapse — 2-7 days repair
- **Flooding:** Water damage — 1-3 weeks repair
- **Wind Storm:** Bridge damage — 3-5 days repair
- **Predator:** Rope/wood damage — 1-2 days repair
- **Fire:** Structure loss — Rebuild needed

<div class='example'>

##### Running Environmental Hazards
When environmental hazards strike:
1. Roll on appropriate table or choose based on story
2. Give players warning based on detection method
3. Set evacuation/response difficulty
4. Apply environmental modifiers to all checks
5. Track infrastructure damage for long-term effects

Remember: Environmental hazards create opportunities for heroism, not just danger. Focus on rescues, protecting others, and community response.
</div>

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

# Social Mechanics

## Reputation System

Track reputation with different factions using a simple scale:

### Reputation Levels
- **Hostile (-3):** Actively opposed, will attack on sight
- **Unfriendly (-2):** Distrusted, increased difficulties
- **Neutral (-1 to +1):** Standard interactions
- **Friendly (+2):** Trusted, reduced difficulties, minor favors
- **Allied (+3):** Strong relationship, major favors, protection

### Key Factions

#### The Five Burrows
- **Mousehattan** - Corporate oligarchy and financial power
- **The Branchx** - Union democracy and working-class solidarity  
- **The Hives** - Cooperative consensus and agricultural innovation
- **Lin's Brook** - Guild confederation and practical expertise
- **Scurry Island** - Survival hierarchy and frontier independence

#### Major Crime Families
- **The Longtail Family** - Old mouse money and traditional crime (Mousehattan)
- **The Whisker Family** - New rat entrepreneurs and modern rackets (Mousehattan)
- **The Silverclaw Family** - Waterfront protection and smuggling (Lin's Brook)
- **The Shadow Runners** - Black market operations and information brokerage (Scurry Island)

#### The Ranger Corps
- **Scurry Island Rangers** - Elite military protecting against titans and external threats

At character creation, players must choose:
- **One faction at -2 reputation** (hostile relationship)
- **One faction at +1 reputation** (friendly relationship)  
- **One faction at +2 reputation** (allied relationship)

\columnbreak

### Detailed Faction Benefits and Consequences

#### The Five Burrows

**Mousehattan - Corporate Oligarchy**
- **Allied (+3):** Access to exclusive financial services, business loans at favorable rates, invitations to high-society events, protection from economic retaliation. Can call upon corporate resources for major favors.
- **Friendly (+2):** Reduced prices at upscale establishments, business networking opportunities, access to financial district information, minor legal assistance.
- **Neutral (0):** Standard business interactions, normal prices and services.
- **Unfriendly (-2):** Increased prices at mouse-owned businesses, difficulty obtaining loans, exclusion from business networks, bureaucratic delays.
- **Hostile (-3):** Economic blacklisting, active sabotage of business ventures, legal harassment, potential violence from crime family associates.

**The Branchx - Union Democracy**
- **Allied (+3):** Full union protection and benefits, priority job placement, access to union legal aid, solidarity during disputes. Can call upon organized labor for strikes or protests.
- **Friendly (+2):** Union job opportunities, discounted services from union members, protection from workplace exploitation, access to worker education programs.
- **Neutral (0):** Standard employment opportunities and workplace treatment.
- **Unfriendly (-2):** Difficulty finding union jobs, higher prices for union services, exclusion from worker solidarity, potential workplace harassment.
- **Hostile (-3):** Blacklisting from union jobs, active sabotage of work projects, physical intimidation, exclusion from working-class communities.

**The Hives - Cooperative Consensus**
- **Allied (+3):** Full community support and resources, access to agricultural innovations, participation in consensus decision-making, protection during crises. Can request community-wide assistance.
- **Friendly (+2):** Preferred access to honey and agricultural products, invitations to community gatherings, assistance with family matters, access to traditional knowledge.
- **Neutral (0):** Standard market prices and community interactions.
- **Unfriendly (-2):** Higher prices for agricultural goods, exclusion from community events, difficulty accessing traditional services, social isolation.
- **Hostile (-3):** Complete social ostracism, denial of essential services, active interference with agricultural needs, potential exile from community areas.

**Lin's Brook - Guild Confederation**
- **Allied (+3):** Master craftsman status and privileges, access to guild secrets and techniques, priority for construction projects, protection of trade interests. Can mobilize guild resources.
- **Friendly (+2):** Apprenticeship opportunities, discounted crafted goods, access to guild workshops, assistance with technical problems.
- **Neutral (0):** Standard prices for crafted goods and services.
- **Unfriendly (-2):** Higher prices for guild services, difficulty accessing quality craftsmanship, exclusion from technical knowledge, delayed project completion.
- **Hostile (-3):** Boycott of services, sabotage of construction projects, denial of essential repairs, potential violence from guild enforcers.

**Scurry Island - Survival Hierarchy**
- **Allied (+3):** Full island protection and resources, access to Ranger training and equipment, safe passage through dangerous areas, emergency assistance. Can call upon island's collective survival expertise.
- **Friendly (+2):** Access to survival training, discounted black market goods, protection during visits, assistance with dangerous situations.
- **Neutral (0):** Standard interactions with island residents and services.
- **Unfriendly (-2):** Higher prices for black market goods, reduced safety during visits, exclusion from survival knowledge, potential targeting by criminals.
- **Hostile (-3):** Active hostility from island residents, denial of safe passage, targeting by criminal elements, potential violence from desperate creatures.

#### Major Crime Families

**The Longtail Family - Traditional Crime**
- **Allied (+3):** Full family protection and resources, access to illegal goods and services, assistance with legal problems, protection from other criminals. Can request family enforcement actions.
- **Friendly (+2):** Reduced "insurance" payments, access to some illegal services, protection from petty crime, assistance with minor legal issues.
- **Neutral (0):** Standard protection racket payments and criminal interactions.
- **Unfriendly (-2):** Increased protection payments, harassment from family associates, difficulty accessing illegal goods, potential targeting for "examples."
- **Hostile (-3):** Active targeting for violence, complete exclusion from criminal services, sabotage of legitimate business, potential assassination attempts.

**The Whisker Family - Modern Rackets**
- **Allied (+3):** Partnership in criminal enterprises, access to advanced criminal techniques, protection from law enforcement, share in family profits. Can request major criminal operations.
- **Friendly (+2):** Favorable terms for illegal services, protection from rival criminals, access to criminal information networks, assistance with law enforcement problems.
- **Neutral (0):** Standard criminal service prices and interactions.
- **Unfriendly (-2):** Higher prices for criminal services, increased scrutiny from family members, potential setup for law enforcement, harassment from associates.
- **Hostile (-3):** Active criminal targeting, sabotage of operations, violence from family enforcers, potential framing for major crimes.

**The Silverclaw Family - Waterfront Crime**
- **Allied (+3):** Control over waterfront operations, access to smuggling networks, protection during water travel, share in smuggling profits. Can mobilize waterfront criminal resources.
- **Friendly (+2):** Safe passage on waterways, access to smuggled goods, protection from water-based threats, assistance with shipping needs.
- **Neutral (0):** Standard waterfront interactions and smuggling prices.
- **Unfriendly (-2):** Harassment during water travel, higher prices for smuggled goods, potential sabotage of water-based activities, exclusion from waterfront areas.
- **Hostile (-3):** Active targeting during water travel, complete exclusion from waterfront, sabotage of boats and water equipment, potential drowning attempts.

**The Shadow Runners - Information Brokers**
- **Allied (+3):** Access to all information networks, protection of personal secrets, assistance with intelligence gathering, share in information profits. Can request major intelligence operations.
- **Friendly (+2):** Access to valuable information, protection of minor secrets, assistance with information needs, favorable terms for intelligence services.
- **Neutral (0):** Standard prices for information and intelligence services.
- **Unfriendly (-2):** Higher prices for information, potential exposure of minor secrets, exclusion from information networks, surveillance and harassment.
- **Hostile (-3):** Active information warfare, exposure of major secrets, complete exclusion from intelligence services, potential blackmail and extortion.

#### The Ranger Corps

**Scurry Island Rangers - Elite Military**
- **Allied (+3):** Full military support and resources, access to advanced weapons and training, protection during titan encounters, emergency evacuation assistance. Can request Ranger intervention in major threats.
- **Friendly (+2):** Basic military training opportunities, access to some Ranger equipment, assistance during emergencies, protection from external threats.
- **Neutral (0):** Standard interactions with military personnel and services.
- **Unfriendly (-2):** Exclusion from military assistance, difficulty accessing Ranger services, potential surveillance, reduced protection during emergencies.
- **Hostile (-3):** Active military opposition, denial of emergency services, potential arrest or detention, targeting as security threat.

<div class='example'>

##### Example Faction Relationships
A **Branchx construction worker** might be **Allied (+3)** with The Branchx union, **Friendly (+2)** with Lin's Brook guilds through work connections, but **Hostile (-3)** to the Longtail Family after refusing to pay protection money and testifying against them.

A **Mousehattan trader** could be **Allied (+3)** with Mousehattan's corporate oligarchy, **Friendly (+2)** with the Whisker Family through business deals, but **Hostile (-3)** to The Hives after a honey price manipulation scandal destroyed several agricultural cooperatives.

A **Scurry Island Ranger** might be **Allied (+3)** with the Ranger Corps, **Friendly (+2)** with Scurry Island's survival hierarchy, but **Unfriendly (-2)** with Mousehattan's corporate interests due to conflicts over resource allocation for titan defense.

</div>

## Economic Status

### Wealth Levels
- **Destitute:** 0-10 acorns, struggling for basic needs
- **Poor:** 11-50 acorns, working class, paycheck to paycheck
- **Comfortable:** 51-200 acorns, stable middle class
- **Wealthy:** 201-1000 acorns, business owners, professionals
- **Rich:** 1001+ acorns, old money families, crime bosses

### Economic Opportunities
- **Day Labor:** 5 acorns per day, no security
- **Skilled Work:** 10-20 acorns per day, union protection
- **Professional Services:** 25-50 acorns per day, requires reputation
- **Business Ownership:** Variable income, requires investment
- **Criminal Activity:** High risk, high reward

<div class='example'>

##### Reputation in Action
Marcus the rat courier has been doing jobs for the Whisker Family, raising his reputation with them from Neutral to Friendly (+2). This gives him access to some illegal services and protection from petty crime.

However, his growing crime family connections have made him Unfriendly (-2) with the legitimate Branchx unions, who suspect he's working for the bosses who exploit workers.

</div>

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

# The Branchx - The Canopy Commons

High above the forest floor, where ancient oaks and maples create a natural metropolis of branches and hollows, The Branchx sprawls through the canopy like a three-dimensional maze of working-class pride and territorial ambition.

## Geography & Infrastructure

### The Vertical Territory
- **The Ancient Grove:** Five massive oaks and seven grand maples form the core
- **Branch Levels:** Seven distinct heights, from "Ground Scrape" to "Crown Touch"
- **The Squirrel Highways:** Major branches worn smooth by generations of travel
- **Hollow Neighborhoods:** Natural tree cavities expanded into communities
- **The Gap:** Dangerous open space between tree clusters, crossed by bridges

### Canopy Architecture
- **Nest Complexes:** Woven structures anchored to major branches
- **Bridge Network:** 47 major crossings, hundreds of minor ones
- **Vertical Territories:** Each family controls trunk-to-crown rights in their tree
- **Emergency Descents:** Bark-stripped slides for rapid evacuation

\columnbreak

### Districts

#### Old Grove Heights *(Traditional Power)*
Highest branches of the Ancient Grove. Multi-generational squirrel families with the best acorn access and winter sun.

#### Working Branch *(Industrial Center)*
Mid-level branches dense with construction staging areas, rope workshops, and union halls.

#### The Tangles *(Dense Neighborhoods)*
Where secondary branches create maze-like communities. Chipmunk courier stations and cheap nest rentals.

#### Ground Scrape *(Lower Levels)*
Just above predator reach. Recent immigrants and struggling families maintaining constant vigilance.

#### New Growth *(Gentrifying Edge)*
Young trees being developed with Mousehattan money creating conflicts over development rights.

#### The Crow Zones *(Rough Territory)*
Branches too close to crow nests. Gang territories with complex relationships with corvids.

## Predator Reality & Defense

### Aerial Threats
- **Hawks:** Daytime terror, forcing covered travel
- **Owls:** Night shift's nightmare, silent death
- **Crows:** Sometimes allies, sometimes threats, always complicated
- **Snakes:** Climbing varieties create seasonal panic

### Defense Systems
- **The Watch:** Rotating sentries with alarm calls
- **Overhead Cover:** Woven canopies over major routes
- **Crow Negotiations:** Protection deals with corvid gangs
- **The Screamers:** Chipmunks whose only job is alarm calls

### Cultural Impact
- **Never Travel Alone:** Buddy system ingrained from birth
- **Branch Patterns:** Routes memorized to avoid open sky
- **Peak Hours:** Dawn and dusk are "death times"
- **The Taken:** Memorial walls for those lost to hawks

<div class=\"footnote\">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

## Demographics & Culture

### Population Breakdown
- **60% Squirrels:** Traditional majority, various subspecies
- **25% Chipmunks:** Essential courier class
- **10% Flying Squirrels:** Elite transport and message services
- **3% Mice:** Usually Mousehattan gentrifiers or climbers
- **2% Others:** Including reformed rats, adventurous voles

### The Families and Gangs

#### The Nutcracker Union
Not just labor - includes "muscle" for disputes. Controls who works construction with "Break more than nuts" reputation.

#### The Tailwind Gang
Chipmunk-dominated courier collective controlling prime message routes. "Neither hawk nor storm" motto.

#### Crow-Affiliated Groups
- **The Black Feathers:** Young squirrels working with crows
- **Shiny Things:** Stealing for corvid bosses
- **The Murder Boys:** Most violent gang

#### Traditional Families
- **The Oakheart Clan:** Oldest squirrel lineage
- **Swiftbranch Dynasty:** Flying squirrel elite
- **The Mapleseed Collective:** Progressive coalition

\columnbreak

<div class='note'>

#### <u>Branchx Sayings</u>

- "High branch, warm winter" (elevation equals security)
- "Every bridge sways" (nothing is certain)
- "Nuts before glory" (practical priorities)
- "The hawk's shadow" (constant danger)
- "Branch born, sky sworn" (pride in canopy life)
- "Splinters build character" (hard work virtue)

</div>

## Daily Life & Economy

### Work Culture
- **Dawn Patrol:** Checking overnight damage
- **Shift Whistles:** Work organized by sun position
- **Sunset Scramble:** Racing darkness home
- **Night Shift:** Dangerous but better paid

### Traditional Industries
- **Construction:** THE identity of The Branchx
- **Acorn Harvesting:** Seasonal boom economy
- **Rope Making:** From spider silk to bark fiber
- **Bridge Building:** Specialized engineering knowledge
- **Courier Services:** Speed is money

### Underground Economy
- **Crow Market:** Goods "fallen off branches"
- **Protection Rackets:** Safety from aerial threats
- **Tunnel Smuggling:** Using abandoned maintenance sections
- **Height Papers:** Fake documents for branch access

<div class='example'>

##### Living in The Branchx
A typical squirrel construction worker starts with Dawn Patrol checking overnight storm damage. Work crews gather at Shift-Change Square when the dawn whistle sounds. Lunch happens on designated "Lunch Branches" for social hour. The sunset scramble home requires checking the sky for predators before making the final sprint to safety.

</div>

<div class=\"footnote\">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

# The Hives - The Crossroads Community

Sprawling across the meadow clearings where forest meets grassland, The Hives earned its name from the dense, interconnected burrow complexes that honeycomb the rolling hills. This is The Great Burrow's most diverse community, where prairie dogs from the southern grasslands live next to mountain marmots, where traditional rabbit warrens neighbor innovative guinea pig terraces.

## Geography & Infrastructure

### The Crossroads Location
- **Gateway Hills:** Rolling terrain that naturally funnels trade routes from the southern grasslands
- **The Convergence:** Where multiple streams meet, creating natural stopping points for caravans
- **Meadow Flats:** Open areas perfect for markets, festivals, and temporary camps
- **Burrow Heights:** Terraced hillsides packed with multi-family housing complexes
- **The Commons:** Central gathering spaces shared by multiple neighborhoods

### Transportation Hub
- **Caravan Grounds:** Staging areas where external traders set up temporary camps
- **The Great Interchange:** Where three Underground lines converge in a massive station
- **Wagon Ways:** Wide paths designed for heavy freight from distant communities
- **The Sorting Yards:** Warehouse district where goods are processed and distributed

### Districts

#### Central Commons *(The Heart)*
The Great Interchange Underground station, multi-cultural markets and food courts, community meeting halls and event spaces.

#### Meadow Heights *(Established Families)*
Traditional rabbit warrens with honey operations. Multi-generational family compounds and conservative community leadership.

#### Grassland Quarter *(Prairie Immigrants)*
Prairie dog settlements with distinctive architecture, wide communal burrow systems, and democratic town-hall style governance.

#### Innovation District *(Mixed Community)*
Guinea pig agricultural experiments, cross-cultural fusion workshops, and experimental housing cooperatives.

\columnbreak

## Demographics & Culture

### Population Breakdown
- **20% Rabbits:** Established families, traditional honey operations
- **18% Prairie Dogs:** Grassland immigrants, community organizers
- **15% Voles & Field Mice:** Working class, service industries
- **12% Guinea Pigs:** Agricultural innovators, recent immigrants
- **10% Marmots:** Mountain immigrants, craftscreatures and builders
- **8% Hamsters:** Merchant families, storage and logistics
- **7% Hedgehogs:** Night shift workers, entertainment industry
- **5% Shrews:** Insect specialists, technical workers
- **5% Mixed/Other:** Various species in smaller numbers

<div class='note'>

#### <u>Hives Sayings</u>

- "Every creature finds their place in the swarm" (everyone belongs somewhere)
- "Many burrows, one community" (unity in diversity)
- "The hive remembers all its workers" (honoring everyone's contributions)
- "Sweet as cooperation" (highest compliment for working together)
- "Different flowers, same garden" (diversity creating beauty)

</div>

## Economy & Daily Life

### Primary Industries
- **Logistics & Distribution:** 30% of burrow economy - processing goods from external trade
- **Small Manufacturing:** 25% - textiles, crafts, household goods, food processing
- **Agriculture & Food:** 20% - honey, grains, specialty foods, fusion cuisine
- **Services:** 15% - restaurants, shops, repair services, cultural businesses
- **Transportation:** 10% - caravan support, Underground operations, courier services

### Cultural Fusion
- **Language Mixing:** Common Forest dialect with words from multiple regions
- **Fusion Cuisine:** Traditional recipes adapted with new ingredients and techniques
- **Hybrid Celebrations:** Festivals combining elements from different cultures
- **Cross-Cultural Learning:** Skills and knowledge exchange between communities

<div class=\"footnote\">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

### The Diversity Council
**Representation:** Delegates from each major community group
**Consensus Building:** Decision-making through discussion and compromise
**Cultural Mediation:** Resolving conflicts between different traditions

### Community Organizations
- **Neighborhood Associations:** Local governance for specific districts
- **Cultural Societies:** Preserving and promoting specific traditions
- **Worker Cooperatives:** Democratic workplace organization
- **Youth Councils:** Representing younger generation interests
- **Elder Circles:** Wisdom and guidance from experienced community members

\columnbreak

<div class='example'>

##### Living in The Hives
The day begins with Dawn Markets where fresh goods arrive via Underground from other burrows. The Great Interchange buzzes with commuters heading to work while caravans arrive from distant communities. Evening brings community meals where different cultural traditions blend in neighborhood gathering spaces.

</div>

### Notable Locations
- **The Great Hall:** Multi-purpose space for large gatherings and celebrations
- **The Exchange:** Central marketplace for local and imported goods
- **Caravan Square:** Staging area for external traders and travelers
- **The Harmony Theater:** Performance space showcasing multiple cultural traditions
- **The Integration Center:** Services for newcomers and cultural orientation

### Challenges & Opportunities
**Integration Tensions:** Cultural preservation vs. adaptation, economic competition between established families and newcomer entrepreneurs

**Growth Opportunities:** Cultural innovation from community mixing, economic diversification, and regional leadership in inter-community cooperation

<div class=\"footnote\">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

# Lin's Brook - The Working Waterfront

Where Whisker Creek meets the tidal waters, Lin's Brook sprawls along both banks in a maze of dams, lodges, and waterfront industry. This is the burrow that builds The Great Burrow - from the wooden frameworks that support tunnels to the boats that brave the rivers.

## Geography & Infrastructure

### The Waterscape
- **Whisker Creek:** The lifeblood, flowing from the northern forests to join the East River
- **The Tidal Reach:** Where creek meets river, creating daily rhythm of high/low water
- **Mill Falls:** Three sets of beaver-engineered drops powering workshops
- **The Wetlands:** Marshy edges where specialized communities thrive
- **Mud Flats:** Exposed at low tide, rich gathering grounds

### Dam Infrastructure
- **The Great Dam:** Master work of beaver engineering, creates the Mill Pond
- **Secondary Dams:** Seven smaller structures controlling flow and creating neighborhoods
- **Lodge Complexes:** Multi-family structures built into dam faces
- **Emergency Breaks:** Designed to fail safely during giant events

### Districts

#### Old Damside *(Historic Heart)*
Original beaver settlement around the Great Dam. Multi-generational lodge complexes with traditional workshops and sawmills.

#### Otter's Landing *(Waterfront Commerce)*
Docks, warehouses, and trading posts. Otter-run ferry terminals with competitive slide-racing venues.

#### The Mills *(Industrial Center)*
Water-powered workshops, lumber processing, and craftscreature quarters with apprentice dormitories.

#### Greenbank *(Gentrifying Waterfront)*
Former industrial areas becoming "artisanal" with converted warehouses housing galleries and rising rents.

\columnbreak

## Water & the Giants

### Aquatic Titans
- **Moose:** Wade through during summer, devastating dam systems
- **Bears:** Fish during salmon runs, entire burrow potentially evacuates
- **Deer:** Crossing at fords causes tsunami-like waves
- **Beavers' Revenge:** Legendary giant beaver that supposedly protects the burrow

### Flood Protocols
- **The Warning Slaps:** Tail-slapping signals travel upstream
- **High Ground Caches:** Emergency supplies above flood lines
- **Sacrificial Dams:** Built to break and dissipate giant-caused waves
- **The Deep Lodges:** Reinforced underwater shelters

<div class='note'>

#### <u>Lin's Brook Sayings</u>

- "Still water, strong dam" (patience and solid work)
- "Every tide turns" (situations change)
- "Swim with the current, build against it" (know when to fight)
- "Wet fur, warm heart" (hard workers are good creatures)
- "The creek provides" (gratitude for resources)
- "Splinters before whiskers" (work comes first)

</div>

## Demographics & Economy

### Population Breakdown
- **35% Beavers:** The founding creatures and infrastructure masters
- **30% Otters:** Waterfront workers and fishercreatures
- **15% Muskrats:** Marsh dwellers and small-craft builders
- **10% Mice/Voles:** Dry-land workers and merchants
- **5% Frogs/Toads:** Newest arrivals, underwater specialists
- **5% Others:** Including some reformed "river rats"

<div class=\"footnote\">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

### Traditional Industries
- **Construction:** Still builds most of Great Burrow's infrastructure
- **Fishing:** Daily catches feed the entire city
- **Lumber:** Sustainable harvesting of storm-fall and dead wood
- **Transportation:** Ferries, cargo hauling, river guides
- **Water Management:** Selling expertise to other burrows

### The Families and The Waterfront

#### River Rat Syndicate
- **The Silverclaw Family:** Controls north dock protection
- **Downstream Boys:** Salvage rights and smuggling
- **The Wet Whiskers:** Gambling boats and fight clubs
- **Code of the Current:** "What sinks stays sunk"

#### Otter Clan Rivalries
Ancient fishing territory disputes, slide-racing betting rings, ferry route monopolies. The Riverclaw vs. Shellcracker feud spans generations.

#### Beaver Lodge Politics
Which families get prime dam positions, construction contract bid-rigging, maintenance fund skimming. "Lodge Law" supersedes burrow rules.

\columnbreak

<div class='example'>

##### Living in Lin's Brook
Work follows the tide schedule - high tide for water work, low tide for maintenance. Dawn brings the best fishing before the city wakes. Mill shifts mean constant operation thanks to water power. Evening markets buzz when the day's catch comes in, while night work on dam repairs happens when water's calmest.

</div>

### Daily Life & Culture

#### Work Rhythms
- **Tide Schedule:** High tide for water work, low tide for maintenance
- **Dawn Fishing:** Best catches before the city wakes
- **Mill Shifts:** Water power means constant operation
- **Evening Markets:** When the day's catch comes in

#### Food Culture
- **Fresh Fish:** Dozen ways to prepare, strong opinions on each
- **Smokehouse Traditions:** Each family guards their wood blend
- **Honey-Smoked Fish:** Premium product using Hives honey
- **Fermented Fish:** Acquired taste, marks true locals

### Notable Locations
- **The First Dam:** Now a monument and museum
- **Shellcracker's Dock:** Otter-run, busiest ferry terminal
- **The Waterlogged:** Dockworker tavern, otter-dominated
- **Slide Stadium:** Professional racing venue
- **The Sunken Lodge:** Underwater meeting place for shady deals

<div class=\"footnote\">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

# External Relations

While The Great Burrow dominates the central forest region, it exists within a broader world of woodland settlements, distant communities, and unexplored territories. These relationships shape trade routes, immigration patterns, diplomatic alliances, and existential threats.

## Trade Relationships

### The Pine Barrens Confederation *(Western Frontier)*
**Primary Species:** Pine martens, porcupines, northern squirrel subspecies
**Trade Goods:** 
- **Exports to Great Burrow:** Pine nuts, resin, winter furs, medicinal bark, survival gear
- **Imports from Great Burrow:** Honey, manufactured goods, acorn products, metal tools

**Relationship:** Cautious but profitable. Pine Barrens creatures are traditional and suspicious of urban ways but need sophisticated products. Trade requires Ranger escorts due to dangerous routes.

### Meadowbrook Settlements *(Southern Grasslands)*
**Primary Species:** Prairie dogs, ground squirrels, rabbit communities
**Trade Goods:**
- **Exports to Great Burrow:** Grains, grassland herbs, woven grass goods, dried flowers
- **Imports from Great Burrow:** Tree nuts, wooden tools, manufactured goods, construction expertise

**Relationship:** Friendly and regular. Strong cultural ties with The Hives through immigration and shared democratic traditions.

### Coastal Tidepools *(Eastern Seaboard)*
**Primary Species:** Crabs, sea otters, coastal mice
**Trade Goods:**
- **Exports to Great Burrow:** Salt, seaweed, shells, dried fish, pearls
- **Imports from Great Burrow:** Fresh water, forest foods, manufactured goods, honey

**Relationship:** Irregular but valuable. Small, scattered communities make trade logistics difficult. Weather and tides affect reliability.

\columnbreak

## The Outlaw Problem

### Bandit Territories *(The Lawless Zones)*
Areas between established settlements where civilization has broken down. Composed of exiles, failed Rangers, desperate creatures, and those who choose the outlaw life.

### Major Bandit Groups
- **The Broken Claw Gang:** Led by disgraced badger, controls mountain passes
- **Whisker's Crew:** Rat-dominated caravan robbery specialists
- **The Feral Pack:** Mixed species "gone wild," most dangerous
- **Shadow Runners:** Sophisticated protection and guide services

### Operations
- **Caravan Raiding:** Primary income from valuable trade goods
- **False Guide Services:** Leading travelers safely, then robbing them
- **Protection Rackets:** "Insuring" safe passage for payments
- **Smuggling Networks:** Moving contraband between settlements

<div class='note'>

#### <u>Trade Route Security</u>

Bandit activity forces expensive Ranger escorts, creates longer "safe routes," drives up import prices, and limits small trader operations. The Great Burrow maintains diplomatic relationships for prisoner exchanges and safe passage negotiations.

</div>

## Diplomatic Relations

### Regional Alliances
- **Oakenheart Alliance:** Forest communities mutual defense pact
- **Meadow Compact:** Southern grassland trade and cultural agreement
- **Waterway Accords:** River and coastal navigation rights

### Immigration Patterns
**Economic Migrants:** Seeking opportunities in The Great Burrow's economy
**Refugees:** Fleeing titan encounters, bandit raids, or community conflicts
**Skilled Workers:** Recruited for specialized knowledge or abilities
**Cultural Immigrants:** Joining established diaspora communities

<div class=\"footnote\">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

# Food & Cuisine

Food in The Great Burrow is culture, politics, economics, and identity all rolled into one. From the 47 traditional ways to prepare acorns to the controversial rise of fusion restaurants, food tells the story of a city where ancient traditions meet urban innovation.

## Traditional Species Cuisines

### Mouse Cuisine *(Refined & Precise)*
**Philosophy:** "Perfection through precision" - every ingredient measured, every technique refined over generations

**Signature Dishes:**
- **Wall Street Cheese Soufflé:** Aged cheese from secret family recipes, served only in financial district
- **Tunnel Dust Crackers:** Incredibly thin, crispy wafers showcasing technical skill
- **Seven-Seed Symphony:** Complex dish requiring exact timing and temperature control
- **Whisker Tea:** Delicate herbal blend served with elaborate ceremony

**Cooking Methods:** Micro-preparation with detailed knife work, aging techniques using wall cavities, precise temperature control with firefly warmth, layered flavor profiles

### Rat Cuisine *(Bold & Abundant)*
**Philosophy:** "More is more" - big flavors, generous portions, fusion experimentation

**Signature Dishes:**
- **Dockside Stew:** Hearty mix of whatever's available, changes daily
- **Spice Route Nuts:** Heavily seasoned with imported spices
- **Entrepreneur's Breakfast:** Massive meal designed to fuel long work days
- **New Money Nachos:** Layered dish showing off expensive imported ingredients

### Squirrel Cuisine *(Seasonal & Stored)*
**Philosophy:** "Prepare for winter" - preservation, storage, and seasonal abundance

**Signature Dishes:**
- **Acorn Mash Supreme:** Ultimate comfort food with 47 traditional preparation methods
- **Winter Cache Casserole:** Layered dish using preserved ingredients
- **Branch-Smoked Nuts:** Nuts smoked with specific woods for distinct flavors
- **Height Celebration Feast:** Elaborate meal served at different canopy levels

\columnbreak

### Beaver Cuisine *(Hearty & Practical)*
**Philosophy:** "Fuel for work" - substantial, nutritious meals providing energy for physical labor

**Signature Dishes:**
- **Dam Builder's Breakfast:** Massive morning meal with bark bread, fish, and nuts
- **Lodge Pot Roast:** Slow-cooked communal meal for extended families
- **Bark Bread Varieties:** Different tree barks create distinct flavors
- **Tail Slap Soup:** Rich broth traditionally shared after construction projects

### Otter Cuisine *(Fresh & Playful)*
**Philosophy:** "Fresh from the water" - emphasis on immediate consumption and social dining

**Signature Dishes:**
- **Sliding Fish:** Fresh catch prepared at the waterfront
- **Ferry Lunch:** Portable meals for workers
- **Splash Party Spreads:** Communal dining with games
- **Current Cocktails:** Fish-based broths and water drinks

<div class='note'>

#### <u>The Acorn Standard</u>

Acorns serve as both primary currency and staple food. The 47 traditional preparation methods include: roasted, ground into flour, aged in oak chambers, fermented into alcoholic beverages, pressed for oils, and combined with honey for preservation. Quality and preparation method affect both nutritional value and exchange rate.

</div>

## Food Politics & Economics

### Honey Monopolies *(The Hives)*
Rabbit families control honey production, creating economic and political tensions. Premium honey commands high prices while basic honey is regulated for fair distribution.

### Seasonal Economics
- **Spring:** Fresh herbs and early nuts, high prices for winter stores
- **Summer:** Peak abundance, preservation activities, competitive harvesting
- **Autumn:** Harvest season, acorn futures markets, storage preparation
- **Winter:** Preserved foods, imported goods, high prices for fresh items

<div class=\"footnote\">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

# The Great Underground

The marvel of mole engineering, this subway system connects all five burrows through natural tunnels, hollow logs, and carved passages.

## Network Overview

### Main Lines

**Red Line: Mousehattan � The Branchx**
- Travel Time: 15 minutes express, 25 minutes local
- Frequency: Every 5 minutes during peak hours
- Challenges: Root interference, seasonal flooding

**Blue Line: Mousehattan � Lin's Brook**
- Travel Time: 20 minutes express, 35 minutes local
- Frequency: Every 8 minutes during peak hours
- Challenges: Water seepage, tidal variations

**Green Line: Mousehattan � The Hives**
- Travel Time: 20 minutes express, 35 minutes local
- Frequency: Every 8 minutes during peak hours
- Challenges: Heavy caravan traffic, diverse passenger needs

**Orange Line: Scurry Island Connection**
- Travel Time: Variable (depends on ferry service and flooding)
- Frequency: Irregular, weather dependent
- Challenges: Frequent flooding, ferry breakdowns, isolation

### Major Stations

#### Grand Central Burrow *(Mousehattan Hub)*
- **Platforms:** 8 platforms serving all major lines
- **Daily Traffic:** 50,000+ passengers
- **Features:** Shopping, dining, information services
- **Architecture:** Carved into the Trading Oak's root system

#### The Great Interchange *(The Hives)*
- **Platforms:** 6 platforms, major multi-line hub
- **Daily Traffic:** 35,000+ passengers
- **Features:** Multi-cultural markets, caravan coordination center
- **Special:** Multi-lingual signage, cargo handling facilities

\columnbreak

## Engineering Marvels

### Mole Engineering Techniques
- **Natural Tunnel Expansion:** Working with existing animal burrows
- **Root Integration:** Building around rather than through tree roots
- **Drainage Systems:** Sophisticated water management
- **Ventilation Networks:** Air circulation using natural pressure differences

### Construction Challenges
- **Giant Footprint Damage:** Tunnels must withstand titan encounters
- **Seasonal Flooding:** Spring runoff and storm drainage
- **Root Growth:** Living trees constantly changing tunnel shapes
- **Predator Infiltration:** Keeping dangerous creatures out

### Rolling Stock and Operations

#### Train Types
- **Express Cars:** Streamlined for speed, limited stops
- **Local Cars:** Frequent stops, larger capacity
- **Cargo Cars:** Freight transport, off-peak hours
- **Emergency Cars:** Medical and disaster response

#### Power Systems
- **Mole Power:** Teams of moles provide propulsion
- **Gravity Assist:** Downhill sections for energy efficiency
- **Mechanical Advantage:** Pulley and lever systems
- **Emergency Backup:** Manual push systems for breakdowns

<div class='note'>

#### <u>Underground Culture</u>

The Great Underground has developed its own culture and etiquette. Commuters form regular social groups, route loyalty is common, and there's an unwritten code of mutual protection during travel.

The system operates 18 hours a day, with reduced service during mole hibernation periods in winter.

</div>

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

# Mousehattan - The Vertical Metropolis

Rising from a rocky outcropping where ancient oak roots penetrate stone, Mousehattan is the beating heart of commerce and ambition. The Acorn Exchange trading floor, carved into the base of the Trading Oak, sets prices that ripple across the forest.

## Geography & Districts

### The Vertical City
- **The Rock:** Natural granite outcropping with chambers carved over generations
- **The Great Oaks:** Three massive ancient oaks whose roots penetrate the rock
- **Root Highways:** Oak roots create natural "avenues" running through stone
- **The Carved Levels:** Seven distinct vertical zones, from Sub-Basement to Crown Level

### Major Districts

#### Wall Street *(Financial District)*
Literally carved into the main rock wall beneath the Trading Oak. Home to the Acorn Exchange and major trading houses with ancient counting rooms using notched-stick tallying systems.

#### Times Squeak *(Entertainment District)*
Where five major tunnels converge beneath interlocking roots. Features 24-hour activity with performance spaces, taverns, and famous roasted seed vendors.

#### The Upper East Roots *(Old Money Residential)*
Carved into the most stable oak root systems. Multi-generation family warrens with private entrances and the exclusive Acorn Club.

#### The Village Burrows *(Bohemian Quarter)*
Maze-like informal tunnels housing artists and radicals. Cheapest rents but most "character," including underground printing presses and The Crumb gathering spot.

## Crime and Order

### The Rat Syndicate *(Primary Organized Crime)*
- **The Longtail Family:** Controls waterfront smuggling
- **The Whisker Brotherhood:** Runs protection rackets
- **The Gray Coats:** Newest family, challenging old territories

\columnbreak

### Crime Culture
- **"The Family Provides":** Code ensuring protection for those who pay
- **Tail Cutting:** Ultimate punishment for betrayal
- **The Bite:** Protection money paid monthly
- **Tunnel Wars:** Territorial disputes resolved underground

### The Underground Economy
- "Insurance" payments are a way of life
- Gambling and illegal seed trade
- Information brokerage through weasel networks
- Black market goods moving through hidden channels

## Daily Life

### Work Culture
- Dawn to past dusk standard for financial sector
- The Acorn Bell signals market open and close
- Whisker Break: Traditional mid-morning grooming/networking
- Complex social hierarchies based on address level

### Dealing with Giants
- Monthly evacuation drills for titan encounters
- The Hush: Children trained to freeze when warning bells ring
- Offering stations maintained to divert giant attention
- "Giant Insurance" is major business, often crime-family run

<div class='note'>

#### <u>Mousehattan Sayings</u>

- "If you can make it here, you can make it anywhere"
- "Every acorn has two sides"
- "The oak remembers"
- "Giants walk where they will" (some things can't be controlled)
- "Connected from root to crown" (having protection)
- "The family provides" (mafia-related)

</div>

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

# Adventure Themes and Hooks

## Urban Survival
Focus on daily challenges of city life, economic pressures, and community building. Adventures involve housing crises, job disputes, and neighborhood problems.

### Sample Adventures
- **The Rent Crisis:** Gentrification threatens to displace a traditional neighborhood
- **Union Strike:** Workers organize against exploitative bosses
- **The Newcomers:** Immigrant community faces discrimination and adaptation challenges
- **Predator in the Pipes:** Dangerous creature infiltrates the Underground system

## Political Intrigue
Emphasize burrow politics, species relationships, and power struggles. Adventures involve elections, policy debates, and factional conflicts.

### Sample Adventures
- **The Disputed Election:** Allegations of voting fraud in Branchx union elections
- **Underground Railroad:** Helping creatures escape crime family debts
- **The Titan Response Debate:** Political fight over defense spending priorities
- **Diplomatic Crisis:** Trade dispute threatens inter-burrow relationships

## Environmental Crisis
Highlight titan threats, predator encounters, and natural disasters. Adventures involve evacuation procedures, infrastructure protection, and survival challenges.

### Sample Adventures
- **The Approaching Giant:** Deer heading toward the city during harvest season
- **The Great Flood Returns:** Spring flooding threatens infrastructure
- **Predator Pack:** Coordinated snake attacks in the canopy
- **The Lost Rangers:** Rescue mission into titan territory

## Social Justice
Explore inequality, workers' rights, and community organizing. Adventures involve union organizing, fighting gentrification, and protecting vulnerable creatures.

### Sample Adventures
- **The Whistleblower:** Exposing corruption in city government
- **Strike Breakers:** Crime families interfering with labor organizing
- **The Housing Fight:** Community resisting luxury development
- **Equal Access:** Ensuring transportation serves all neighborhoods

\columnbreak

## Crime and Family Business
Navigate the complex world of organized crime, family loyalty, and moral choices in the shadows of the city.

### Sample Adventures
- **Family War:** Conflict between Longtail and Gray Coats families
- **The Inside Job:** Someone's skimming from protection money
- **Going Legitimate:** Crime family member trying to escape "the life"
- **The Double Agent:** Weasel selling information to multiple families

<div class='example'>

##### Adventure Hook: The Missing Messenger
**Setup:** A chipmunk courier carrying important documents between burrows has disappeared. The package contained contracts for a major construction project that could reshape the city's infrastructure.

**Complications:** 
- Multiple crime families want the contracts
- Union organizers suspect corporate sabotage  
- The courier's family fears the worst
- Titans have been spotted near the usual delivery routes

**Resolution:** Characters must investigate the disappearance, navigate criminal and political interests, and either rescue the courier or recover the documents - all while dealing with the dangerous forces that may have caused the disappearance.

</div>

<div class='note'>

#### <u>Campaign Themes</u>

The Great Burrow works best when adventures connect to the larger themes of urban life, cooperation vs. competition, and the daily heroism of small creatures building something larger than themselves.

Characters should feel like they're part of a living city where their actions matter and where every adventure contributes to the ongoing story of creatures trying to build civilization in a dangerous world.

</div>

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

## Burrow-Specific Adventures

### Mousehattan Hooks
- **The Acorn Exchange Crash:** Market manipulation threatens to destroy the economy. Characters must uncover the conspiracy before financial collapse ruins thousands.
- **The Wall Rights War:** Ancient mouse families fight over prime territory while new construction threatens historical chambers. Legal battles turn violent.
- **Times Squeak Scandal:** The newspaper prepares to expose crime family secrets. Characters must protect journalists or silence them, depending on loyalties.

### The Branchx Hooks  
- **The Failed Tunnel Mystery:** Strange sounds emerge from the abandoned tunnel project. Workers report missing tools and eerie lights in the depths.
- **Corvid Politics:** The crow allies demand increased territory in exchange for continued protection. Negotiations could reshape the canopy.
- **Union Corruption:** The Nutcracker Union leadership may be taking bribes. A reformer needs protection during election season.

### The Hives Hooks
- **The Beetle Uprising:** Overworked insects begin refusing commands. Without them, the agricultural system faces collapse.
- **Trade Route Bandits:** Prairie dog merchants report increased attacks. Someone is organizing the outlaws with inside information.
- **The Democratic Crisis:** Vote tampering in the Hive Mind councils threatens to tear apart the cooperative consensus.

\columnbreak

### Lin's Brook Hooks
- **Dam Sabotage:** Critical infrastructure failures suggest deliberate damage. If the Great Dam fails, the entire burrow loses power.
- **The Fixed Races:** Otter slide-racing championships show signs of crime family interference. Gambling debts turn deadly.
- **Gentrification Wars:** Craft breweries and artisan shops displace working families. Violence erupts between old-timers and newcomers.

### Scurry Island Hooks
- **Ranger Recruitment:** Characters must prove themselves worthy to join the elite titan-fighters. Training involves real danger.
- **The Old Giant's Secret:** Deep exploration of the fallen oak reveals pre-city artifacts. What did the Rangers' founders hide?
- **Black Market War:** Competing factions fight for control of smuggling routes. Neutral parties get caught in the crossfire.

## Cross-Burrow Adventures

### The Great Underground Collapse
A section of tunnel between Mousehattan and The Hives collapses during rush hour. Characters must:
- Navigate dangerous detours while helping trapped commuters
- Investigate whether this was accident or sabotage
- Deal with political fallout as burrows blame each other
- Race against time before air runs out for survivors

### The Inter-Burrow Serial Killer
Someone is targeting specific species across multiple burrows. Characters must:
- Navigate different burrow jurisdictions and politics
- Profile a killer who knows the Underground perfectly
- Protect potential victims while hunting the predator
- Uncover the dark secret connecting all victims

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

## Seasonal Campaign Seeds

### Spring Adventures
- **The Flood Conspiracy:** Someone's redirecting flood waters to destroy specific neighborhoods. Environmental warfare meets urban politics.
- **Mating Season Madness:** Hormone-driven violence threatens the peace. Traditional courtship competitions turn into gang warfare.
- **The Lost Kits:** Spring births lead to missing children. Is it predators, titans, or something worse taking the young?

### Summer Adventures
- **The Tourist Trap:** Visitors from distant forests bring exotic problems. Cultural misunderstandings escalate to international incidents.
- **Heat Wave Hallucinations:** Extreme temperatures cause mass visions. Are they heat-induced or is something supernatural occurring?
- **The Drought War:** Water becomes more valuable than acorns. Control of streams and wells sparks burrow conflicts.

### Fall Adventures
- **Harvest Heist:** Someone's systematically stealing winter stores. Without reserves, thousands will starve.
- **The Early Winter:** Premature cold threatens unprepared communities. Characters race to secure emergency supplies.
- **Festival Sabotage:** The Harvest Gratitude celebration faces disruption. Political messages through violent means.

### Winter Adventures
- **The Heating Crisis:** Fuel shortages create desperate measures. Crime families control warmth distribution.
- **Cabin Fever:** Isolated communities develop strange beliefs. Cult activity increases during the darkest months.
- **The Ice Bridge:** Frozen rivers create new titan paths. Emergency evacuation plans need immediate implementation.

\columnbreak

## Long Campaign Arcs

### The Titan Prophecy (15-20 sessions)
Ancient writings suggest titans will converge on the city during a specific celestial alignment. Characters must:
- Decipher pre-city texts and symbols
- Navigate religious and scientific communities
- Prepare defenses without causing panic
- Confront the truth about titan intelligence

**Campaign Themes:** Faith vs. reason, community preparation, ancient mysteries

### The Underground Empire (25-30 sessions)
Discovery of vast pre-Burrow ruins beneath the city reveals an earlier civilization. Characters explore:
- Lost technology and knowledge
- Dangerous guardians and traps
- Political implications of the discovery
- The reason the previous city fell

**Campaign Themes:** Progress vs. tradition, hidden history, power of knowledge

### The Species Integration Movement (20-25 sessions)
Young creatures push for radical equality, challenging traditional hierarchies. Characters navigate:
- Peaceful protests turning violent
- Generational conflicts within families
- Economic disruption from social change
- Outside agitators with hidden agendas

**Campaign Themes:** Social justice, generational change, price of progress

### The Economic Revolution (30-40 sessions)
The acorn standard collapses, threatening civilization. Characters must:
- Investigate market manipulation
- Prevent food riots and social collapse
- Design new economic systems
- Balance competing burrow interests

**Campaign Themes:** Economic inequality, innovation vs. stability, community survival

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

# GM Guidance

## Tone and Atmosphere
- **Cozy but Dangerous:** The city is home, but threats are real
- **Community Focused:** Individual success tied to group welfare
- **Working Class Heroes:** Characters are ordinary creatures doing extraordinary things
- **Urban Fantasy:** Magic is cooperation, technology is ingenuity
- **Hope and Struggle:** Challenges are serious but not insurmountable

## NPC Motivations
- **Survival:** Basic needs, safety, security
- **Community:** Family, species, burrow loyalty
- **Ambition:** Economic advancement, political power
- **Tradition:** Preserving old ways, cultural identity
- **Progress:** Innovation, integration, modernization

## Conflict Sources
- **Economic:** Inequality, gentrification, resource scarcity
- **Cultural:** Species integration vs. traditional hierarchies
- **Environmental:** Titan threats, predator encounters, weather
- **Political:** Burrow autonomy vs. city unity
- **Personal:** Family obligations vs. individual dreams

## Success Metrics
Success in The Great Burrow isn't just about individual achievement, but about strengthening community bonds, protecting vulnerable creatures, and building a better city for everyone.

Measure success by:
- **Community Impact:** How actions affect neighborhoods and burrows
- **Relationship Building:** Strengthening bonds between different groups
- **Problem Solving:** Creative solutions to urban challenges
- **Cultural Preservation:** Maintaining traditions while embracing change
- **Collective Prosperity:** Ensuring benefits reach all creatures

\columnbreak

<div class='note'>

#### <u>Scale and Perspective</u>

Never forget that these are small creatures in a big, dangerous world. A house cat is a kaiju-level threat. A dropped human wallet could fund an entire neighborhood. The constant awareness of scale should influence every aspect of play.

This vulnerability breeds both caution and audacity - creatures who build subway systems and skyscrapers while knowing that a single giant footstep could destroy everything they've built.

</div>

<div class='note wide'>

#### <u>Managing the Five Burrows</u>

Each burrow has its own personality, challenges, and opportunities. Don't try to develop all five equally in every campaign - focus on 2-3 burrows that interest your players most, while keeping the others as background elements that occasionally influence events.

**Mousehattan** works for corporate intrigue and crime family drama. **The Branchx** suits working-class heroes and union stories. **The Hives** excels at community cooperation and cultural exchange. **Lin's Brook** provides infrastructure challenges and practical problem-solving. **Scurry Island** offers frontier adventure and military action.

Let the players' backgrounds and interests guide which burrows become central to your campaign.

</div>

<div class='example'>

##### Bringing the City to Life
**Environmental Details:** The constant sound of tiny feet on wooden walkways, the scent of roasted seeds from street vendors, the play of filtered sunlight through leaves overhead.

**Cultural Touches:** Chipmunks speaking in rapid courier slang, mice discussing market fluctuations in precise terms, the rumble of the Underground train carrying workers home.

**Daily Challenges:** Checking the sky for predators before leaving cover, timing commutes around titan warning systems, navigating the complex social networks that determine who gets which opportunities.

These details make The Great Burrow feel like a real place where real creatures live, work, and dream.

</div>

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

<div class="note wide">

#### <u>Quick Reference Tables</u>

##### Seasonal Challenges

- **Spring:** Environmental: Flooding, construction season — Social: Mating season tensions — Economic: Building boom, trade revival
- **Summer:** Environmental: Heat, drought, peak titans — Social: Tourism, social events — Economic: Peak trading, water costs
- **Autumn:** Environmental: Storms, preparation pressure — Social: Harvest celebrations — Economic: Economic boom, hoarding
- **Winter:** Environmental: Cold, limited travel — Social: Family gatherings, strain — Economic: Food scarcity, high costs

##### Titan Encounter Responses

- **Bear:** 30 minutes warning — City-wide evacuation — 2-6 hours duration
- **Deer:** 60 minutes warning — Affected districts evacuation — 1-3 hours duration
- **Moose:** 2+ hours warning — Regional evacuation — 4-12 hours duration
- **Wild Boar:** 15 minutes warning — Local areas evacuation — 30 minutes-2 hours duration

##### Crime Family Territory

- **Longtail:** Mousehattan — Traditional protection — Honor, respect
- **Whisker:** Mousehattan — Modern rackets — Business, profit
- **Silverclaw:** Lin's Brook — Waterfront, smuggling — Practical, direct
- **Shadow Runners:** Scurry Island — Black market, information — Survival, pragmatic

</div>

##### Adventure Complications

- **2-3:** Titan spotted approaching the area
- **4-5:** Predator attack disrupts plans
- **6-7:** Weather turns dangerous
- **8-9:** Crime family gets involved
- **10-11:** Union strike affects transportation
- **12:** Government investigation launched

\columnbreak

##### Random Encounters

- **2-3:** Underground: Tunnel flooding — Surface: Hawk patrol — Canopy: Bridge maintenance
- **4-5:** Underground: Train breakdown — Surface: Giant footprint — Canopy: Nest robbers
- **6-7:** Underground: Lost tourist — Surface: Market crowd — Canopy: Rope bridge traffic
- **8-9:** Underground: Crime family meeting — Surface: Street performance — Canopy: Squirrel territory dispute
- **10-11:** Underground: Mole strike — Surface: Courier race — Canopy: Construction accident
- **12:** Underground: Emergency evacuation — Surface: Titan offering ceremony — Canopy: Crow gang recruitment

<div class='read'>

*"The Great Burrow never sleeps. From the pre-dawn preparation of seed vendors to the after-midnight meetings in hidden speakeasies, this city pulses with the energy of creatures who refuse to be small. Every tunnel tells a story, every bridge represents a dream made real, and every citizen embodies the audacious spirit that built civilization in the shadow of giants."*

From "A Newcomer's Guide to The Great Burrow" by Scholar Brightwhisker

</div>

Welcome to The Great Burrow - where every dawn brings opportunity and danger in equal measure, where your burrow shapes your identity but doesn't define your destiny, and where small creatures with enormous dreams prove every day that size isn't what matters - it's what you build together.

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

# Quick Reference Tables

## Common Sayings by Burrow

### Mousehattan
- "If you can make it here, you can make it anywhere"
- "Every acorn has two sides"
- "The oak remembers"
- "Connected from root to crown" (having protection)
- "The family provides" (mafia-related)

### The Branchx
- "High branch, warm winter" (elevation equals security)
- "Every bridge sways" (nothing is certain)
- "Nuts before glory" (practical priorities)
- "The hawk's shadow" (constant danger)
- "Splinters build character" (hard work virtue)

### The Hives
- "Every creature finds their place in the swarm"
- "Many burrows, one community" (unity in diversity)
- "Sweet as cooperation" (highest compliment)
- "Different flowers, same garden" (diversity creating beauty)

### Lin's Brook
- "Still water, strong dam" (patience and solid work)
- "Every tide turns" (situations change)
- "Swim with the current, build against it"
- "Wet fur, warm heart" (hard workers are good)
- "Splinters before whiskers" (work comes first)

### Scurry Island
- "Play dead 'til you're ready" (strategic patience)
- "Every ferry's the last" (appreciate what comes)
- "Rangers lead, shadows follow" (respect and secrecy)
- "West is death, east is debt" (trapped between dangers)

\columnbreak

## Acorn Economy Price Guide

### Basic Currency
- **1 Acorn Cap:** Small daily purchase (newspaper, snack)
- **1 Whole Acorn:** Meal at modest restaurant
- **5 Acorns:** Day's wages for unskilled labor
- **10 Acorns:** Week's groceries for single creature
- **50 Acorns:** Month's rent in working-class neighborhood
- **100 Acorns:** Quality winter coat
- **500 Acorns:** Small nest/burrow down payment
- **1,000 Acorns:** Modest family home
- **5,000+ Acorns:** Prime territory rights

### Seasonal Price Fluctuations
- **Spring:** Prices 20% higher (winter stores depleted)
- **Summer:** Stable prices, luxury goods available
- **Autumn:** Harvest season, prices drop 30%
- **Winter:** Essential goods 50% higher, luxury scarce

<div class='note wide'>

#### <u>Random Encounters by Burrow</u>

##### Mousehattan (d12)
1. Crime family "tax collector"
2. Acorn Exchange insider information
3. Lost tourist needs directions
4. Street performer entertaining crowd
5. Pickpocket attempts theft
6. Wealthy mouse drops valuable item
7. Underground newspaper vendor
8. Firefly maintenance overhead
9. Business argument spills public
10. Misdirected courier message
11. Giant warning evacuation drill
12. Crime family war erupts

##### The Branchx (d12)
1. Hawk forces creatures to cover
2. Bridge inspection reveals danger
3. Union organizer recruiting
4. Chipmunk courier urgent message
5. Construction accident blocks route
6. Crow demands safe passage tribute
7. Gentrification protesters march
8. Young squirrel rescue needed
9. Family feud blocks crossing
10. Storm damage dangerous conditions
11. Gang territory markers appear
12. Predator alarm from watch posts

##### The Hives (d12)
1. Bee swarm escapes, causes panic
2. Guinea pig innovation demonstration
3. Traditional vs. modern farming argument
4. Beetle workforce strikes
5. Honey shipment "falls off wagon"
6. Night market firefly malfunction
7. Agricultural inspector violations
8. Inter-species cultural celebration
9. Shrew commands confuse insects
10. Free-range advocate vandalism
11. Rare flower unusual insects
12. Harvest festival chaos

</div>

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

# Governance & Politics

The Great Burrow operates under a complex system that balances burrow autonomy with city-wide cooperation.

## The Inter-Burrow Council

### Structure and Powers
- **Composition:** Two representatives from each burrow (10 total)
- **Meeting Location:** Rotates between burrows quarterly
- **Powers:** Infrastructure funding, titan response, inter-burrow disputes, trade regulation
- **Limitations:** Cannot override burrow-specific laws or cultural practices

### Current Representatives
- **Mousehattan:** Councilmouse Goldwhisker (old money), Councilrat Steeltail (new money)
- **The Branchx:** Councilsquirrel Oakheart (traditional), Councilchipmunk Swiftstripe (union)
- **The Hives:** Councilrabbit Honeycomb (agricultural), Councilpig Whistlebelly (innovation)
- **Lin's Brook:** Councilbeaver Strongdam (builders), Councilotter Shellcracker (dockworkers)
- **Scurry Island:** Councilpossum Deadtail (old families), Ranger-Commander Scarback (military)

## Individual Burrow Systems

### Mousehattan - Corporate Oligarchy
- **The Root Board:** Informal council of family heads and crime bosses
- **Acorn Exchange Authority:** Financial market regulation
- **District Wardens:** Appointed local management
- **Law:** "What's good for business is good for the burrow"

### The Branchx - Union Democracy
- **Nutcracker Assembly:** Union and family representatives
- **Height Council:** Traditional squirrel ceremonial roles
- **Tail Vote:** Direct democracy by literally raising tails
- **Law:** "Every creature earns their perch"

### The Hives - Democratic Consensus
- **Diversity Council:** Multi-community representation
- **Species Circles:** Internal group governance
- **The Forum:** Town-hall style meetings
- **Law:** "Every creature finds their voice in the swarm"

\columnbreak

### Lin's Brook - Guild Confederation
- **Dam Council:** Guild representatives
- **Water Rights Court:** Ancient stream access management
- **Tide Speakers:** Elected neighborhood positions
- **Law:** "Strong dams, fair currents"

### Scurry Island - Survival Hierarchy
- **Trunk Council:** Whoever maintains order and respect
- **Ranger Command:** Military authority during titan threats
- **Sanctuary Keepers:** Neutral safe zone enforcement
- **Law:** "Survive first, argue later"

<div class='note'>

#### <u>Political Movements</u>

**The Traditionalists:** Preserve burrow autonomy and species-specific governance
**The Unionists:** Worker rights and cross-species solidarity  
**The Progressives:** Modernization and technological advancement
**Rangers First:** Titan defense and military preparedness
**The Naturalists:** Environmental protection and sustainable development

</div>

## Current Political Crises

### The Infrastructure Question
- Aging Great Underground needs massive investment
- Competing proposals for funding and management
- Political fight over construction contracts

### The Titan Response Debate
- Increasing giant activity near the city
- Ranger expansion vs. civilian evacuation improvements
- Religious movements claiming giants are angry about growth

### Economic Inequality
- Wealth gap between burrows growing
- Gentrification displacing traditional communities
- Debate over minimum wage and worker protections

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

# Organized Crime & The Underworld

Crime in The Great Burrow operates as a parallel economy and shadow government, providing services the legal system cannot or will not offer.

## The Rat Syndicates *(Mousehattan)*

### The Longtail Family *(Traditional Power)*
- **Territory:** Lower Mousehattan, waterfront smuggling
- **Leadership:** Don Salvatore "Big Sal" Longtail
- **Specialties:** Protection rackets, loan sharking, tunnel smuggling
- **Code:** "The family provides" - honor-based obligations
- **Allies:** Traditional mouse families, conservative business interests
- **Enemies:** The Gray Coats, reform movements

### The Whisker Brotherhood *(New Money)*
- **Territory:** Financial district, new developments
- **Leadership:** Capo Regina "Whiskers" McGillicuddy  
- **Specialties:** Business fraud, gambling, real estate schemes
- **Code:** "Make holes bigger" - expansion at any cost
- **Allies:** Rat entrepreneurs, corrupt officials
- **Enemies:** Longtail traditionalists, union organizers

### The Gray Coats *(Rising Power)*
- **Territory:** Times Squeak, entertainment districts
- **Leadership:** Boss Tommy "Gray Tail" Rattington
- **Specialties:** Entertainment rackets, drug trade, youth recruitment
- **Code:** "New city, new rules" - rejecting old ways
- **Allies:** Young creatures, progressive businesses
- **Enemies:** Both established families, law enforcement

## Regional Crime Operations

### The Silverclaw Family *(Lin's Brook)*
- **Territory:** Waterfront, ferry operations
- **Leadership:** Mother Marta Silverclaw (ancient otter)
- **Specialties:** Smuggling, dock worker protection, ferry "insurance"
- **Operations:** Less subtle than Mousehattan families, more blue-collar
- **Code:** "Wet paws, clean money" - honest work when possible

### The Shadow Runners *(Scurry Island)*
- **Territory:** Black markets, Ranger recruitment
- **Leadership:** The Council of Masks (anonymous leaders)
- **Specialties:** Contraband trading, document forging, exile services
- **Operations:** Most sophisticated fence operations in the city
- **Code:** "What's lost stays lost" - perfect operational security

\columnbreak

<div class='note'>

#### <u>Crime Family Services</u>

**Protection Rackets:** Often provide actual security from worse threats
**Loan Sharking:** Financial services for creatures banks won't serve
**Dispute Resolution:** Faster than legal courts, enforceable results
**Black Market Goods:** Items not available through legal channels
**Information Brokerage:** Intelligence networks spanning the city
**Smuggling Operations:** Moving goods past regulations and taxes

</div>

## Criminal Hierarchies and Codes

### Family Structure
- **Don/Boss:** Family head, makes major decisions
- **Underboss:** Second in command, daily operations  
- **Consigliere:** Advisor, dispute mediation
- **Capo:** Lieutenant, territory management
- **Soldier:** Made member, enforcement
- **Associate:** Works with family, not full member

### The Criminal Economy
- **Territory Rights:** Families respect each other's areas
- **The Accommodation:** Police understand some crime is inevitable
- **Information Trade:** Knowledge as valuable as goods
- **Recruitment Patterns:** Desperate creatures, family connections
- **Tribute Systems:** Everyone pays someone for protection

### Notable Criminal Enterprises
- **The Floating Casino:** Gambling boat moving between jurisdictions
- **The Tunnel Express:** Smuggling network using abandoned subway routes
- **The Night Markets:** Black market goods sold after legitimate businesses close
- **The Document Mills:** False identification and citizenship papers
- **The Giant Insurance Scam:** Fake titan damage claims

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

# Technology & Innovation

## Insect-Based Technology

The Great Burrow's technology relies on cooperation with non-sapient insects rather than mechanical devices.

### Agricultural Systems
- **Beetle Farming:** Managed beetle colonies for soil aeration and waste processing
- **Bee Partnerships:** Honey production through carefully maintained hive relationships  
- **Ant Labor:** Organized ant colonies for construction and transportation
- **Silkworm Operations:** Spider silk production for rope and fabric manufacturing

### Communication Technology
- **Messenger Services:** Trained beetles for package delivery
- **Signal Networks:** Cricket orchestras for long-distance communication
- **Emergency Systems:** Firefly networks for warning signals
- **Information Processing:** Ant-based counting and calculation systems

### Transportation Innovation
- **Underground Propulsion:** Mole-powered train systems
- **Cargo Networks:** Beetle-drawn cart systems
- **Emergency Transport:** Bat courier services for urgent needs
- **Water Transport:** Beaver-engineered boats and ferry systems

### Construction Technology
- **Web Architecture:** Spider silk structural engineering
- **Living Buildings:** Growing structures using trained plant growth
- **Water Management:** Beaver dam engineering principles
- **Excavation Systems:** Coordinated burrowing using multiple species

\columnbreak

<div class='note'>

#### <u>Innovation Centers</u>

**The Hives Innovation District:** Cross-cultural fusion of techniques
**Mousehattan Engineering Firms:** Precision manufacturing and finance tech
**Lin's Brook Workshops:** Practical construction and water management
**Branchx Construction Cooperatives:** Democratic technology development
**Scurry Island Survival Tech:** Improvised solutions for extreme conditions

</div>

## Economic Innovation

### Financial Systems
- **Acorn Standardization:** Quality grading and exchange rate management
- **Credit Systems:** Reputation-based lending across burrows
- **Investment Cooperatives:** Community-owned business development
- **Insurance Markets:** Risk pooling for titan encounters and disasters
- **Trade Documentation:** Standardized contracts and shipping manifests

### Manufacturing Advances
- **Assembly Line Production:** Multi-species collaborative manufacturing
- **Quality Control:** Species-specific expertise ensuring standards
- **Specialization Networks:** Burrow-based production advantages
- **Distribution Systems:** Underground and surface logistics coordination

## Social Innovation

### Community Organization
- **Democratic Innovations:** New forms of consensus-building across species
- **Conflict Resolution:** Inter-species mediation and justice systems
- **Education Systems:** Multi-cultural learning environments
- **Integration Programs:** Supporting immigrant and refugee communities

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

# Religion & Spirituality

## Major Spiritual Traditions

### The Old Growth Faith
- **Core Belief:** The forest as a living entity with consciousness and will
- **Sacred Sites:** Ancient trees, especially the Trading Oak and the Old Giant
- **Practices:** Tree meditation, root reading, bark offerings
- **Clergy:** Grove Keepers (usually badgers and older squirrels)
- **Holy Days:** First Leaf (spring awakening), Root Deep (autumn grounding)

### The Great Harmony
- **Core Belief:** All creatures interconnected in cosmic balance
- **Sacred Sites:** The Great Interchange, multi-species gathering places
- **Practices:** Multi-species meditation circles, cooperative work as worship
- **Clergy:** Harmony Speakers (diverse species, elected positions)
- **Holy Days:** Unity Dawn (summer solstice), Balance Night (autumn equinox)

### The Titan Mysteries
- **Core Belief:** Giants carry divine messages and spiritual power
- **Sacred Sites:** Titan footprints, offering stations, survivor monuments
- **Practices:** Dream interpretation, offering ceremonies, survival rituals
- **Clergy:** Oracle-Survivors (creatures who've encountered titans directly)
- **Holy Days:** Giant's Rest (whenever titans are spotted), Memorial of the Taken

### The Deep Current *(Lin's Brook Tradition)*
- **Core Belief:** Water as spiritual life force connecting all things
- **Sacred Sites:** The Great Dam, spring sources, tidal pools
- **Practices:** Tide meditation, water blessing ceremonies, flow readings
- **Clergy:** Current Readers (beavers and otters with spiritual calling)
- **Holy Days:** Spring Flow (flood season), Deep Water (winter ice)

\columnbreak

### The Great Burrow *(Urban Spirituality)*
- **Core Belief:** The city itself as sacred achievement of cooperation
- **Sacred Sites:** Grand Central Burrow, construction sites, union halls
- **Practices:** Building blessings, innovation worship, community service
- **Clergy:** Work Blessed (craftscreatures recognized for spiritual dedication)
- **Holy Days:** Foundation Day (city anniversary), Builder's Rest (construction season end)

### The Shadow Path *(Scurry Island)*
- **Core Belief:** Accepting harsh realities while maintaining dignity and hope
- **Sacred Sites:** The Ranger Memorial, Root Town sanctuaries, exile shrines
- **Practices:** Survival meditation, ancestor honoring, truth telling
- **Clergy:** Shadow Speakers (usually opossums and reformed criminals)
- **Holy Days:** Night of Truths (winter solstice), Dawn of Chances (spring equinox)

<div class='note'>

#### <u>Religious Tensions & Cooperation</u>

**Syncretism:** Many creatures blend traditions, especially immigrants
**Seasonal Cooperation:** Joint celebrations during city-wide festivals  
**Political Influence:** Religious leaders often mediating disputes
**Titan Response:** Competing approaches to giant encounters
**Social Justice:** Religious movements supporting workers' rights and equality

</div>

## Spiritual Practices in Daily Life

### Community Rituals
- **Morning Blessings:** Work crews starting with brief spiritual moments
- **Meal Sharing:** Religious significance of communal dining
- **Crisis Response:** Spiritual leaders coordinating disaster relief
- **Life Transitions:** Birth, naming, coming of age, partnership, death ceremonies

### Personal Spirituality
- **Meditation Practices:** Species-specific spiritual disciplines
- **Seasonal Observances:** Individual marking of natural cycles
- **Ancestor Veneration:** Honoring family and species heritage
- **Vision Quests:** Young creatures seeking spiritual direction

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

# External Relations & Trade

## Regional Trading Partners

### The Pine Barrens Confederation *(Western Frontier)*

<div class='note'>

#### <u>Trade Profile</u>

**Distance:** 3-day journey by caravan, weather permitting
**Population:** ~15,000 creatures across scattered settlements
**Government:** Loose confederation of family territories
**Primary Species:** Pine martens, porcupines, northern squirrel subspecies

</div>

**Exports to Great Burrow:**
- Pine nuts and conifer seeds (winter staples)
- Medicinal bark and forest remedies
- Resin for waterproofing and preservation
- Winter furs and cold-weather gear
- Survival equipment and wilderness guides

**Imports from Great Burrow:**
- Honey and agricultural products
- Manufactured goods and metal tools
- Acorn products and tree nuts
- Construction expertise and engineering

**Relationship Status:** Cautious but profitable. Pine Barrens creatures are traditional and suspicious of urban ways but need sophisticated products. Trade requires Ranger escorts due to bandit activity on routes.

### Meadowbrook Settlements *(Southern Grasslands)*

**Exports to Great Burrow:**
- Grains and grass seeds
- Grassland herbs and medicinal plants
- Woven grass goods and textiles
- Dried flowers and prairie specialties

**Imports from Great Burrow:**
- Tree nuts and forest products
- Wooden tools and construction materials
- Manufactured goods and honey
- Engineering expertise for irrigation

**Relationship Status:** Friendly and regular. Strong cultural ties with The Hives through immigration and shared democratic traditions. Seasonal trading expeditions bring cultural exchange.

\columnbreak

### Coastal Tidepools *(Eastern Seaboard)*

**Exports to Great Burrow:**
- Salt for preservation and trade
- Seaweed and ocean vegetables
- Shells for decoration and tools
- Dried fish and seafood delicacies
- Pearls and rare ocean finds

**Imports from Great Burrow:**
- Fresh water (precious on coast)
- Forest foods and tree products
- Manufactured goods and honey
- Underground engineering expertise

**Relationship Status:** Irregular but valuable. Small, scattered communities make trade logistics difficult. Weather and tides affect reliability. High value, low volume transactions.

## The Bandit Problem

### Major Outlaw Groups

**The Broken Claw Gang**
- **Leader:** "Iron Back" Grimjaw (disgraced badger)
- **Territory:** Mountain passes between Pine Barrens and Great Burrow
- **Specialty:** Caravan ambushes, protection rackets
- **Size:** ~50 members, seasonal recruitment

**Whisker's Crew**
- **Leader:** "Fast Tooth" Ratsby (rat entrepreneur gone wrong)
- **Territory:** Southern trade routes to Meadowbrook
- **Specialty:** Sophisticated robbery, false guide services
- **Size:** ~30 members, highly mobile

**The Feral Pack**
- **Leader:** Unknown (rumors of a "gone wild" fox)
- **Territory:** Northern wastes, titan territory
- **Specialty:** Extreme violence, trophy taking
- **Size:** ~20 members, most dangerous

### Bandit Economics
- Force expensive Ranger escorts for valuable shipments
- Create longer "safe routes" that increase transport costs
- Drive up import prices through supply disruption
- Limit small trader operations to established routes only

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

# Master Timeline

## The Founding Era *(150-120 Years Ago)*

### The Great Convergence *(150 Years Ago)*
A series of disasters forced scattered settlements to unite: the Terrible Winter that lasted 8 months, multiple bear encounters destroying isolated communities, harvest failures, and the Great Storm that devastated traditional territories. Survivors gathered at the current site of The Great Burrow.

### The Acorn Compact *(148 Years Ago)*
Legendary agreement establishing principles of mutual aid, shared defense, and peaceful dispute resolution. Created the foundation for inter-species cooperation and the basic legal framework still used today.

### First Infrastructure *(145-130 Years Ago)*
- **The Great Underground:** Initial tunnel system connecting major settlements
- **Bridge Networks:** Canopy connections enabling The Branchx development
- **Water Management:** Early dam systems creating Lin's Brook as viable community
- **The Trading Oak:** Establishment of central commerce and government

## Growth and Crisis *(120-60 Years Ago)*

### The Species Wars *(82-76 Years Ago)*
Economic inequality and cultural conflicts erupted into the most serious internal strife in city history. Traditional mouse families clashed with emerging rat entrepreneurs, while working-class species fought against both. Resolution came through the Great Compromise establishing current burrow autonomy system.

### The Great Compromise *(76 Years Ago)*
- Established the Five-Burrow system with significant autonomy
- Created the Inter-Burrow Council for city-wide coordination
- Recognized species-specific governance while maintaining city unity
- Set precedent for democratic participation across species lines

### The Great Flood *(59 Years Ago)*
Catastrophic flooding caused by unusual spring conditions and upstream giant activity. Demonstrated both city vulnerability and resilience, leading to improved emergency planning, infrastructure hardening, and social welfare programs.

\columnbreak

## The Modern Era *(60 Years Ago-Present)*

### Innovation Period *(45-30 Years Ago)*
- **Insect Agriculture Revolution:** Guinea pig innovations transforming food production
- **Transportation Improvements:** Expansion of Great Underground system
- **Cross-Species Integration:** Increasing cooperation and intermarriage
- **Economic Diversification:** Growth beyond traditional species-based occupations

### Prosperity Decades *(30-10 Years Ago)*
- **Regional Dominance:** The Great Burrow becomes major cultural and economic center
- **Population Growth:** Immigration from across the forest region
- **Infrastructure Expansion:** Modern transportation and communication systems
- **Cultural Renaissance:** Arts, entertainment, and education flourishing

### Current Challenges *(10 Years Ago-Present)*
- **Gentrification Crisis:** Wealthy interests displacing traditional communities
- **Environmental Pressures:** Increasing titan activity and climate changes
- **Economic Inequality:** Growing wealth gaps testing cooperative principles
- **Political Tensions:** Debates over centralization vs. burrow autonomy

### Recent Major Events

**The Great Trampling *(20 Years Ago)*:** Most destructive single titan encounter in city history. Bear rampage through Mousehattan resulted in major infrastructure damage and evacuation protocol reforms.

**The Ferry Crisis *(5 Years Ago)*:** Complete breakdown of Scurry Island ferry service led to isolation crisis and political tensions over infrastructure investment priorities.

**The Honey Wars *(3 Years Ago)*:** Price manipulation scandal in agricultural markets exposed corruption in Hives governance and led to democratic reforms.

**The Underground Strike *(Last Year)*:** Mole transportation workers organized first city-wide work stoppage, paralyzing Great Underground and forcing negotiations over working conditions.

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

# Index

<div class="wide">

<center>

## Comprehensive Index

</center>

</div>

<div style="margin-top:25px;"></div>

<span class="index-letter">A</span>
<ul class="index">
<li><span>Acorn Economy</span><span>2512</span></li>
<li><span>Adventure Themes</span><span>2250</span></li>
<li><span>Arts & Entertainment</span><span>1044</span></li>
</ul>

<span class="index-letter">B</span>
<ul class="index">
<li><span>Badgers</span><span>Additional Species</span></li>
<li><span>Beavers</span><span>820</span></li>
<li><span>The Branchx</span><span>1538, 677</span></li>
</ul>

<span class="index-letter">C</span>
<ul class="index">
<li><span>Careers</span><span>908</span></li>
<li><span>Chipmunks</span><span>793</span></li>
<li><span>Communication Systems</span><span>1113</span></li>
<li><span>Crime & Families</span><span>Organized Crime</span></li>
</ul>

<span class="index-letter">E</span>
<ul class="index">
<li><span>Environmental Rules</span><span>1374</span></li>
<li><span>Equipment & Gear</span><span>1165</span></li>
<li><span>External Relations</span><span>Trade Relations</span></li>
</ul>

<span class="index-letter">F</span>
<ul class="index">
<li><span>Five Burrows Overview</span><span>672</span></li>
<li><span>Food & Cuisine</span><span>2005</span></li>
</ul>

<span class="index-letter">G</span>
<ul class="index">
<li><span>GM Guidance</span><span>2329</span></li>
<li><span>Governance & Politics</span><span>Politics</span></li>
<li><span>Great Underground</span><span>2084</span></li>
<li><span>Guinea Pigs</span><span>866</span></li>
</ul>

\columnbreak

<span class="index-letter">H</span>
<ul class="index">
<li><span>The Hives</span><span>1679, 680</span></li>
</ul>

<span class="index-letter">L</span>
<ul class="index">
<li><span>Lin's Brook</span><span>1797, 683</span></li>
</ul>

<span class="index-letter">M</span>
<ul class="index">
<li><span>Master Timeline</span><span>Timeline</span></li>
<li><span>Mice</span><span>725</span></li>
<li><span>Moles</span><span>Additional Species</span></li>
<li><span>Mousehattan</span><span>2171, 674</span></li>
</ul>

<span class="index-letter">O</span>
<ul class="index">
<li><span>Opossums</span><span>Additional Species</span></li>
<li><span>Organized Crime</span><span>Crime & Underworld</span></li>
<li><span>Otters</span><span>Additional Species</span></li>
</ul>

<span class="index-letter">R</span>
<ul class="index">
<li><span>Rabbits</span><span>842</span></li>
<li><span>Raccoons</span><span>Additional Species</span></li>
<li><span>Random Encounters</span><span>2533</span></li>
<li><span>Rats</span><span>747</span></li>
<li><span>Religion & Spirituality</span><span>Religion</span></li>
<li><span>Reputation System</span><span>1460</span></li>
</ul>

<span class="index-letter">S</span>
<ul class="index">
<li><span>Scurry Island</span><span>686</span></li>
<li><span>Shrews</span><span>Additional Species</span></li>
<li><span>Skills Reference</span><span>984</span></li>
<li><span>Social Mechanics</span><span>1458</span></li>
<li><span>Species as Archetypes</span><span>719</span></li>
<li><span>Squirrels</span><span>771</span></li>
</ul>

<span class="index-letter">T</span>
<ul class="index">
<li><span>Talents</span><span>1306</span></li>
<li><span>Technology & Innovation</span><span>Technology</span></li>
<li><span>Titan Encounters</span><span>1376</span></li>
</ul>

<span class="index-letter">W</span>
<ul class="index">
<li><span>Weasels</span><span>Additional Species</span></li>
</ul>

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum
<style>
    #p17{ display: none;}
</style>
