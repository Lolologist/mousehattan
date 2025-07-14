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

<div class='read'>

*The morning mist rises from the forest floor as the first bell chimes from Mousehattan's Root Cathedral. Across the Great Burrow, ten thousand creatures stir to life. In The Branchx, squirrels leap between rope bridges, their morning chatter mixing with the creak of wood and the distant cry of a hawk. Below, in the Underground tunnels, mole work crews push the first trains of the day through passages that smell of earth and old roots. This is your city—dangerous, beautiful, and alive with possibility.*

</div>

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

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

The giants aren't inherently malevolent - they simply exist at a scale that makes coexistence nearly impossible. The Great Burrow has evolved elaborate warning systems, evacuation protocols, and offering stations to minimize catastrophic encounters.

<div class='note'>

#### <u>Titan Encounter Pacing</u>

Titans should be rare, terrifying events - not regular combat encounters. Use them to:
- Create dramatic evacuation scenes
- Force difficult choices (save the kit or the acorn stores?)
- Drive long-term campaign consequences
- Show community cooperation under pressure

Roll once per season for titan activity, not once per session. When titans appear, make it memorable.

</div>

### Natural Predators
- **Hawks**: Control daytime surface travel, forcing covered routes
- **Owls**: Silent death in the night shift
- **Snakes**: Seasonal terror in the canopy
- **Corvids**: Complex relationship - sometimes protection, sometimes threat

<div class='note'>

#### <u>Running Predator Encounters</u>

When players encounter predators, create tension through:
- **Perception checks** to spot them early
- **Cool checks** to avoid panicking
- **Stealth vs Vigilance** opposed checks
- **Chase scenes** using range bands

Remember: Predators shouldn't be constant combat - they're environmental hazards that shape behavior and create dramatic moments.

</div>

\columnbreak

<div class='note'>

#### <u>Scale and Perspective</u>

Understanding scale is crucial in The Great Burrow. Most playable and encountered species exist at the scale of ~6 inches to perhaps a foot tall. Unlike the size discrepancies of the real world, in The Great Burrow, most creatures have a semi-normalized size. In contrast, the titans - bears, deer, moose - move through the landscape like living natural disasters. 

Yet the creatures of The Great Burrow have built a thriving civilization through cooperation, ingenuity, and sheer audacity. This is a world where being small means thinking big.
</div>

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

## The Five Burrows

### Mousehattan - The Vertical Metropolis

The beating heart of commerce and ambition, carved into a rocky outcropping where ancient oak roots create natural highways. Wall Street is literally carved into walls, while Times Squeak never sleeps under managed firefly lighting. This vertical city rises through seven distinct levels from Sub-Basement to Crown Level, housing 28,000 creatures in a maze of root highways and carved chambers.

**Notable Features:** The Acorn Exchange trading floor built into the Trading Oak's hollow, the Whiskers Building (12 stories of carved stone), Gallery Row displaying rare seeds, and the infamous underground Squeakeasy run by the Longtail crime family. The district operates on "acorn time" with dawn-to-dusk financial markets driving the entire burrow's rhythm.

**Demographics:** 40% mice (old money families), 25% rats (business and crime), 15% voles (middle management), 10% hamsters (merchants), 10% others.

<div class='read'>

*You emerge from the Underground into Times Squeak just as the firefly lanterns flicker to life. The scent of roasted seeds fills your nostrils as vendors hawk their wares. Above, through gaps in the root ceiling, you glimpse the legendary Whiskers Building rising twelve stories of carved stone. A well-dressed mouse brushes past, muttering about acorn futures, while a rat in a sharp vest argues loudly with a beaver in construction garb about "making the hole bigger." Welcome to Mousehattan, where fortunes are made before dawn and lost before dusk.*

</div>

\columnbreak

### The Branchx - The Canopy Commons

<div class='read'>

*The rope bridge sways beneath your paws, a hundred tail-lengths above the forest floor. To your left, a chipmunk courier races past, cheeks bulging with messages, her crew tattoo visible on her shoulder. The afternoon sun filters through leaves, casting everything in green-gold light. From somewhere above comes the rhythmic hammering of the Nutcracker Union at work—building, always building, reaching ever higher. A squirrel matron passes, her tail held high with third-branch pride, while below, new immigrants scramble for space on the dangerous lower levels. This is The Branchx, where height is everything and everyone knows their place.*

</div>

Working-class pride in three-dimensional tree cities spanning fifty massive oaks and seventy grand maples. 47 major rope bridge crossings connect the vertical neighborhoods, while emergency bark slides provide rapid descent during predator attacks. The canopy stretches across seven branch levels from "Ground Scrape" to "Crown Touch," housing 18,000 creatures in nest complexes and hollow expansions.

**Cultural Identity:** Construction IS The Branchx - from the Nutcracker Union that controls building projects to the rope weavers whose craft passes through generations. The failed tunnel system below serves as both reminder of broken promises and convenient smuggling network. Corvid zones add danger where desperate creatures make deals with crow gangs for aerial protection.

**Demographics:** 60% squirrels (traditional majority), 25% chipmunks (courier class), 10% flying squirrels (premium transport), 5% others including mice gentrifiers.

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

### The Hives - The Crossroads Community

<div class='read'>

*The morning caravan bells ring across The Hives as prairie dog sentries announce the arrival of traders from the southern grasslands. In the Great Interchange below, the rumble of Underground trains mingles with a dozen different dialects as commuters rush to work. A rabbit matron haggles in broken Prairie-speak with a guinea pig farmer over terraced vegetables, while her kits play with vole children in the common square. Above it all, the sweet scent of honey drifts from traditional warrens, mixing with exotic spices from the fusion food stalls. This is The Hives - where every creature finds their place in the swarm, and diversity isn't just tolerated but celebrated as the burrow's greatest strength.*

</div>

The Great Burrow's most diverse district, sprawling across meadow clearings where forest meets grassland. This buzzing center of 24,000 creatures earned its name from dense, interconnected burrow complexes honeyccombing the rolling hills. Prairie dog democratic councils share space with traditional rabbit warrens, while guinea pig agricultural terraces demonstrate innovative farming techniques adapted from mountain traditions.

**Economic Hub:** The Great Interchange where three Underground lines converge makes this the logistics capital. 30% of the economy runs on processing external trade, with caravan grounds hosting traders from distant communities. The Sorting Yards warehouse district processes goods from across the forest region, while mixed-species workshops produce fusion crafts combining multiple cultural traditions.

**Cultural Melting Pot:** "Everyone finds their place in the swarm" through cooperation rather than bloodlines. The Integration Center helps newcomers adapt, while cross-cultural families pioneer new ways of living. Night markets buzz with firefly light as creatures enjoy cuisine from across the known world.

\columnbreak

### Lin's Brook - The Working Waterfront


Blue-collar waterfront pride where Whisker Creek meets the East River's tidal waters. The Great Dam powers water-driven workshops through Mill Falls, while seven secondary dams create distinct neighborhoods. This engineering marvel houses 20,000 creatures who know that high tide means water work while low tide brings maintenance and repairs.

**Working Culture:** The Dockworkers Union (otter-dominated) shares power with the Builders Guild (beaver-led but increasingly diverse). Traditional industries like sustainable lumber harvesting and fishing feed the entire Great Burrow, while gentrifying Greenbank converts old warehouses into artisanal workshops - to the disgust of working families priced out of their ancestral lodges.

**Water Life:** Complex tail-slap communications coordinate flood protocols for when titans wade through. The Silverclaw crime family controls north dock "protection" while rival otter clans maintain ancient fishing territory disputes. Every kit learns to read currents before they can properly swim.

<div class='read'>

*The morning shift bell clangs across the waterfront as fog rolls off Whisker Creek. An otter surfaces near the dock, fish writhing in her jaws, while beaver work crews inspect the Great Dam's mighty timbers. The air tastes of salt, sawdust, and honest sweat. A young rat loads cargo, dreaming of something more than dock work, while old-timers mutter about gentrification creeping in from Greenbank. The tide is turning—in more ways than one. This is Lin's Brook, where the water never lies and every creature knows the value of a hard day's work.*

</div>

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum


### Scurry Island - The Forgotten Burrow

<div class='read'>

*The ferry lurches as it approaches Scurry Island's ramshackle dock. Through the mist, you see them—Rangers, standing watch on the Heights, quills and crossbows ready. Below, the Harbor Market sprawls in chaotic glory, where anything can be bought if you know the right creature to ask. An opossum plays dead in an alley while picking pockets. A one-eyed badger spits tobacco juice and sizes you up. "First time on the Island?" she growls. "Then remember the rules: mind your business, pay your debts, and when the titan bell rings—you run like hell or you die standing." Welcome to the last free place in The Great Burrow.*

</div>

Isolated on a true island across dangerous straits, this 10,000-creature community serves as both shadow economy hub and last line of defense against Deep Woods titans. The rocky shores and dense interior provide perfect cover for those seeking to disappear from mainland law. Connected only by three ferries (two usually broken), this is where the desperate, the criminal, and the brave Rangers make their home.

**The Ranger Corps:** Elite scouts operate from fortified Heights overlooking the mainland. Led by a one-eyed badger Watch Commander, they recruit society's desperate to face bears, moose, and worse. Equipment includes poison-tipped porcupine quills, flash powder, and scent bombs. The Wall of the Fallen honors those who stood "between the city and the dark."

**Shadow Economy:** Everything has a price in Harbor Market - from forged documents to concentrated fermented sap. The Fence Lords control major operations while opossum and raccoon families run traditional "businesses." Old Town enforces sanctuary rules even as the Lowland Shanties flood with each storm. Underground fighting pits and gambling dens hide in the Warrens, where "what happens in the deep stays in the deep."

\columnbreak

<div class='note'>

#### <u>Running Scurry Island Adventures</u>

Scurry Island works best when players feel the isolation and danger. Key elements:
- **Ferry Unreliability:** Roll a d6 when players need transport. On 1-2, the ferry is "broken" that day
- **Ranger Respect:** Being a Ranger or having Ranger connections opens doors that money can't
- **Black Market Etiquette:** Everything requires introduction. Cold approaches get cold shoulders (or worse)
- **The Titan Bell:** When it rings, EVERYONE stops what they're doing. Heroes who help during titan emergencies earn deep loyalty
- **Sanctuary Rules:** Even crime bosses respect the sanctuary tradition. Breaking it makes you everyone's enemy

Remember: Scurry Island isn't evil, it's desperate. Most creatures here are survivors, not villains.

</div>

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

# Chapter 1 - Character Creation

## Species as Archetypes

<div class='read'>

*"You can tell everything about a creature by how they enter a room," old Grandmother Hazelnut used to say. And here in The Great Burrow, she was right. Watch the mouse pause at the threshold, checking exits and evaluating everyone's social standing. See the rat burst through, loud and confident, already talking about their next big score. Notice how the squirrel immediately scans for the highest perch, while the beaver examines the craftsmanship of the doorframe. Each species carries ten thousand years of instinct into this modern city—and in a world of giants and predators, those instincts keep you alive.*

</div>

Rather than using traditional fantasy races, characters choose from woodland creature species that function as archetypes, each providing different starting characteristics and special abilities.

<div class='note'>

#### <u>Roleplaying Different Species</u>

Help players embody their species through:
- **Physical mannerisms**: Mice groom whiskers when nervous, rats gesture broadly
- **Speech patterns**: Reference the vocal patterns section
- **Cultural values**: What matters to their species?
- **Instinctive reactions**: Prey species freeze, predator species investigate

Encourage species-specific solutions to problems!

</div>

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
- **Social Networks:** Start with one contact in Mousehattan, and +1 reputation (max of +2 to start)

**Starting Skills:** Choose 2 from: Charm, Deception, Knowledge (City), Mechanics, Negotiation, Streetwise

**Background:** Descendants of the original wall-carvers. Mousehattan IS mouse town in their minds.

\columnbreak 

**Cultural Traits:**
- Obsessed with genealogy and wall-rights dating back generations
- Believe in "proper" ways of doing everything

**Vocal Patterns:** Precise, articulated speech with old-fashioned vocabulary. Use formal titles and proper grammar even in casual conversation. Speak softly but expect to be heard.

**Occupations:** Bankers, lawyers, Wall Street traders, gallery owners, old-school deli operators

**Species Sayings:**
- *"A mouse can nibble through anything, given time"* (persistence wins)
- *"Know your tunnels, know your exits"* (always have a backup plan)
- *"Cheese ages, roots decay"* (some things improve with time, others don't)

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

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

\columnbreak

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

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

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
- **Speed Burst:** Once per session, may move to any location within Medium range as an incidental
- **Cheek Pouches:** Can carry small items without encumbrance penalty
- **Route Knowledge:** Remove <span class='setback'>b</span> from Streetwise checks related to navigation

**Starting Skills:** Choose 2 from: Athletics, Coordination, Perception, Vehicles, Streetwise, Vigilance

**Background:** Fast Branchx couriers, risk-takers who form tight crew families.

**Cultural Traits:** Speed obsessed, proud of cheek-pouch capacity, route efficiency focused, crew loyalty over height status.

**Vocal Patterns:** Rapid-fire delivery with slang and abbreviations. Extensive hand gestures, crew members finish each other's sentences.

**Occupations:** Messengers, couriers, smugglers, tunnel maintenance

**Sayings:** *"Full cheeks, empty promises"* / *"Winter comes for the slow"*

\columnbreak

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
- **Starting XP:** 90

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

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

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

\columnbreak

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
Tedi is creating a mouse character. She takes the mouse archetype (Brawn 1, Agility 2, Intellect 3, Cunning 2, Willpower 2, Presence 2) and decides to play an up-and-coming trader from Mousehattan. She chooses Charm and Negotiation as her starting skills and takes the Acorn Trader career for additional business skills.
</div>

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

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
<span class="bra">3</span>
<span class="agi">1</span>
<span class="int">2</span>
<span class="cun">2</span>
<span class="wil">2</span>
<span class="pre">2</span>
</div>

- **Wound Threshold:** 12 + Brawn
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
<span class="pre">2</span>
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
<span class="bra">2</span>
<span class="agi">2</span>
<span class="int">2</span>
<span class="cun">1</span>
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
<span class="agi">3</span>
<span class="int">2</span>
<span class="cun">2</span>
<span class="wil">1</span>
<span class="pre">3</span>
</div>

- **Wound Threshold:** 8 + Brawn
- **Strain Threshold:** 10 + Willpower
- **Starting XP:** 80

**Special Abilities:**
- **Hyperactive:** May perform second maneuver per turn without strain cost
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
<span class="int">1</span>
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
<span class="cun">3</span>
<span class="wil">1</span>
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
- **Starting XP:** 90

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
- **Starting XP:** 90

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
<span class="bra">1</span>
<span class="agi">3</span>
<span class="int">3</span>
<span class="cun">3</span>
<span class="wil">1</span>
<span class="pre">1</span>
</div>

- **Wound Threshold:** 10 + Brawn
- **Strain Threshold:** 11 + Willpower
- **Starting XP:** 80

**Special Abilities:**
- **Cunning Hunter:** Add <span class='boost'>b</span><span class='boost'>b</span> to Skulduggery and Deception checks
- **Predator Heritage:** Smaller creatures must make Hard <span class='difficulty'>d</span><span class='difficulty'>d</span><span class='difficulty'>d</span> Discipline check when around foxes to avoid intimidation (adding setbacks to their social checks)
- **Quick Thinking:** Once per session, upgrade any skill check twice instead of once when using a story point

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

### Dogs *(The Loyal Companions)*

<div class="archetype">
<span class="bra">2</span>
<span class="agi">2</span>
<span class="int">2</span>
<span class="cun">2</span>
<span class="wil">2</span>
<span class="pre">2</span>
</div>

- **Wound Threshold:** 11 + Brawn
- **Strain Threshold:** 11 + Willpower
- **Starting XP:** 110

**Special Abilities:**
- **Pack Loyalty:** Add <span class='boost'>b</span> to checks when helping allies or defending family
- **Enhanced Senses:** Add <span class='boost'>b</span> to Perception checks using smell or hearing
- **Wolf Heritage:** May cause fear in other creatures; once per encounter, add <span class='boost'>b</span> to Coercion checks

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
<span class="agi">3</span>
<span class="int">2</span>
<span class="cun">2</span>
<span class="wil">1</span>
<span class="pre">3</span>
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
<span class="wil">3</span>
<span class="pre">2</span>
</div>

- **Wound Threshold:** 8 + Brawn
- **Strain Threshold:** 8 + Willpower
- **Starting XP:** 110

**Special Abilities:**
- **Insect Communication:** Can communicate with insects through ultrasonic whistles, add <span class='boost'>b</span><span class='boost'>b</span> to Animal Handling checks with insects
- **Hyperactive Metabolism:** Must eat every 4 hours or suffer strain, but add <span class='boost'>b</span> to Athletics checks
- **Tiny Size:** Add <span class='boost'>b</span><span class='boost'>b</span> to Stealth checks, but increase difficulty of Brawl checks against larger creatures by 1

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

\columnbreak

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


<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum


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
- **Cheek Pouches:** Can carry two items up to Encumbrance 3 in their mouths without penalty
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

**Long-lived Species (20-30+ years):** Beavers, badgers - extensive institutional memory

This creates intergenerational dynamics where longer-lived species serve as mentors and institutional memory, while shorter-lived species drive innovation and change.

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


### Union Organizer
Labor activists working to improve conditions and rights for the city's working creatures.

**Skills:** Charm, Coercion, Leadership, Negotiation, Perception, Streetwise, Knowledge (City), Cool
**Starting Equipment:** Union materials, worker contacts, meeting spaces

### Black Market Dealer
Traders in goods and services that exist outside the legal economy.

**Skills:** Deception, Negotiation, Skulduggery, Streetwise, Vigilance, Knowledge (City), Cool, Perception
**Starting Equipment:** Contraband goods, hidden storage, criminal contacts

<div class='note'>

#### <u>Labor Conflicts as Adventures</u>

Union stories provide non-combat challenges:
- **Negotiation scenes** with management
- **Rally organization** requiring Leadership
- **Strike-breaking** attempts by crime families
- **Sabotage investigations** at work sites
- **Protection** of union leaders from thugs

These create moral dilemmas and social encounters!

</div>


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
- **Animal Handling (Willpower):** Handle non-sapient animals and insects, calm panicked animals
- **Athletics (Brawn):** Climb, swim, jump, run for extended periods
- **Cool (Presence):** Initiative in aware situations, stay calm, gambling, keep nerve
- **Coordination (Agility):** Swing on ropes, walk narrow surfaces, squeeze into spaces, escape restraints
- **Discipline (Willpower):** Confront terror, keep sanity, heal strain, meditate
- **Mechanics (Intellect):** Repair damage, identify parts, design devices, sabotage, build items
- **Medicine (Intellect):** Heal wounds, counteract poison, cure disease, medical procedures
- **Navigation (Intellect):** Read maps, set courses, plot routes under stress
- **Perception (Cunning):** Search for clues, study landscape, conduct surveillance
- **Resilience (Brawn):** Go without sleep, fight off toxins, endure hostile environments
- **Riding (Agility):** Control mounts, mounted combat, 
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

<div class='read'>

*The weapon merchant spreads her wares across the moth-silk cloth. "Mouse-made," she says, lifting a needle sword that gleams with precision, "notice the balance, the engravings—five generations of technique in every fold." She sets it down, picks up a brutal nutcracker club. "Now this—pure Branchx work. Beaver-carved, squirrel-tested, could crack a giant's acorn or a rival's skull." Her raccoon paws dance over the goods with practiced ease. "Everything has its purpose, its maker, its story. The question is—what story do you want to tell?"*

</div>

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

\columnbreak 

### Otter-Made Equipment
- **Modifications:** Waterproof quality, +1 Defense against environmental hazards
- **Price:** +15% (specialized waterproofing)
- **Aesthetics:** Sleek, streamlined design that functions equally well in water and on land. Uses water-resistant materials and sealed construction. Often includes drainage features.

### Rabbit-Made Equipment
- **Modifications:** Add Defensive +1 quality to armor, reduce crafting time by 25%
- **Price:** -10% (community production methods)
- **Aesthetics:** Comfortable, practical design focused on protection and family use. Often includes padding and comfort features. Built for extended wear and community sharing.

### Opossum-Made Equipment
- **Modifications:** equipment appears worthless (Deception bonus for concealment), item always damaged at least one step (cf. CRB p.89, <span class='setback'>b</span> on all checks made with it)
- **Price:** -50% (appears cheap but functions well)
- **Aesthetics:** Deliberately shabby appearance hiding quality construction. Designed to be underestimated. Often incorporates scavenged materials in clever ways.

### Squirrel-Made Equipment
- **Modifications:** Reduce weight by 1 Encumbrance (minimum 0), add Superior quality to climbing gear
- **Price:** Standard
- **Aesthetics:** Lightweight construction using hollow components and flexible materials. Designed for mobility and storage. Often includes attachment points for securing to trees or rope systems.

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

### Chipmunk-Made Equipment
- **Modifications:** Add <span class='boost'>b</span> to Athletics checks when using equipment, reduce size by one category
- **Price:** +10% (specialized for speed and agility)
- **Aesthetics:** Compact, streamlined design optimized for rapid movement. Built-in storage pouches and quick-release mechanisms. Everything designed for courier work.

### Mole-Made Equipment
- **Modifications:** Add <span class='boost'>b</span> to underground Navigation, equipment functions in complete darkness
- **Price:** +20% (specialized underground applications)
- **Aesthetics:** Tactile construction with raised surfaces and texture guides. No visual elements needed. Built for underground durability.

### Skunk-Made Equipment
- **Modifications:** Intimidating, add <span class='boost'>b</span> to Coercion when visible
- **Price:** +25% (reputation and specialized construction)
- **Aesthetics:** Bold black and white design that announces the maker. High-quality construction that commands respect. Often includes warning symbols.

\columnbreak

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

### Brawl Weapons
- **Claw Guards:** Damage +1, Crit 3, Range [Engaged], Encumbrance 1, Price 15 acorns, *Defensive 1*
- **Brass Knuckles:** Damage +1, Crit 4, Range [Engaged], Encumbrance 0, Price 10 acorns, *Disorient 1*
- **Tail Wrap:** Damage +2, Crit 5, Range [Engaged], Encumbrance 1, Price 12 acorns, *Knockdown*
- **Tooth Caps:** Damage +1, Crit 3, Range [Engaged], Encumbrance 0, Price 20 acorns, *Vicious 1*
- **Grappling Claws:** Damage +0, Crit 5, Range [Engaged], Encumbrance 1, Price 18 acorns, *Ensnare 1*
- **Spiked Collar:** Damage +1, Crit 4, Range [Engaged], Encumbrance 1, Price 25 acorns, *Defensive 1*
- **Paw Wraps:** Damage +0, Crit 5, Range [Engaged], Encumbrance 0, Price 8 acorns, *Accurate 1*

### Melee Weapons
- **Sharpened Stick:** Damage +2, Crit 5, Range [Engaged], Encumbrance 1, Price 2 acorns
- **Thorn Spear:** Damage +3, Crit 4, Range [Engaged], Encumbrance 2, Price 5 acorns
- **Needle Sword:** Damage +3, Crit 2, Range [Engaged], Encumbrance 1, Price 35 acorns, *Pierce 1*
- **Nutcracker Club:** Damage +4, Crit 4, Range [Engaged], Encumbrance 3, Price 20 acorns, *Knockdown*
- **Stone Axe:** Damage +5, Crit 3, Range [Engaged], Encumbrance 3, Price 55 acorns, *Vicious 1*
- **Climbing Pick:** Damage +3, Crit 4, Range [Engaged], Encumbrance 1, Price 22 acorns, *Pierce 1, Defensive 1*
- **Beetle Prod:** Damage +2, Crit 5, Range [Engaged], Encumbrance 1, Price 30 acorns, *Stun Damage*
- **Insect Goad:** Damage +1, Crit 6, Range [Engaged], Encumbrance 1, Price 20 acorns, *Stun, Animal Handling <span class='boost'>b</span>*
- **Builder's Hammer:** Damage +3, Crit 4, Range [Engaged], Encumbrance 2, Price 15 acorns, *Disorient 1*
- **Branch Sword:** Damage +4, Crit 3, Range [Engaged], Encumbrance 2, Price 50 acorns, *Defensive 1*
- **Whisker Blade:** Damage +2, Crit 2, Range [Engaged], Encumbrance 0, Price 60 acorns, *Accurate 1, Pierce 1*


<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

### Ranged (Light) Weapons
- **Sling:** Damage 4, Crit 4, Range [Medium], Encumbrance 1, Price 10 acorns
- **Bark Bow:** Damage 5, Crit 3, Range [Long], Encumbrance 2, Price 40 acorns, *Prepare 1*
- **Acorn Sling Staff:** Damage 5, Crit 4, Range [Medium], Encumbrance 2, Price 45 acorns, *Accurate 1*
- **Fishing Spear:** Damage 4, Crit 3, Range [Short], Encumbrance 2, Price 18 acorns, *Accurate 1* (underwater)
- **Rope Dart:** Damage 2, Crit 4, Range [Short], Encumbrance 1, Price 35 acorns, *Ensnare 1, Accurate 1*
- **Thorn Whip:** Damage 2, Crit 4, Range [Short], Encumbrance 1, Price 30 acorns, *Ensnare 1*
- **Seed Shooter:** Damage 3, Crit 5, Range [Medium], Encumbrance 1, Price 25 acorns, *Limited Ammo 3*
- **Blowgun:** Damage 2, Crit 4, Range [Short], Encumbrance 0, Price 30 acorns, *Accurate 2, Poison*
- **Titan Spear:** Damage 5, Crit 3, Range [Medium], Encumbrance 2, Price 80 acorns, *Pierce 2*
- **Poison Dart:** Damage 3, Crit 2, Range [Short], Encumbrance 0, Price 25 acorns, *Poison (stun)*
- **Entanglement Net:** Damage 1, Crit 6, Range [Short], Encumbrance 2, Price 50 acorns, *Ensnare 2*
- **Flash Powder:** Damage 0, Crit -, Range [Short], Encumbrance 1, Price 30 acorns, *Blast 3, Stun*
- **Smoke Bomb:** Damage 0, Crit -, Range [Short], Encumbrance 1, Price 20 acorns, *Blast 2, Disorient 2*
- **Emergency Flare:** Damage 1, Crit 5, Range [Long], Encumbrance 1, Price 15 acorns, *Burn 1, Bright light*
- **Sap Glue Trap:** Damage 0, Crit -, Range [Short], Encumbrance 1, Price 25 acorns, *Immobilize 2*
- **Pinecone Grenade:** Damage 6, Crit 4, Range [Medium], Encumbrance 1, Price 40 acorns, *Blast 4, Limited Ammo 1*

\columnbreak

### Ranged (Heavy) Weapons
- **Ranger Crossbow:** Damage 6, Crit 3, Range [Long], Encumbrance 3, Price 150 acorns, *Accurate 1, Prepare 1*
- **Coal Launcher:** Damage 8, Crit 4, Range [Medium], Encumbrance 4, Price 300 acorns, *Blast 6, Burn 2, Limited Ammo 1, Prepare 2*
- **Bamboo Ballista:** Damage 10, Crit 3, Range [Extreme], Encumbrance 5, Price 500 acorns, *Pierce 4, Breach 1, Limited Ammo 1, Prepare 3, Anti-Titan*
- **Heavy Siege Bow:** Damage 7, Crit 3, Range [Long], Encumbrance 4, Price 200 acorns, *Pierce 2, Prepare 2, Cumbersome 2*
- **Steam Cannon:** Damage 9, Crit 4, Range [Long], Encumbrance 5, Price 400 acorns, *Blast 5, Concussive 1, Limited Ammo 2, Prepare 2*
- **Porcupine Quill Launcher:** Damage 7, Crit 2, Range [Long], Encumbrance 3, Price 250 acorns, *Pierce 3, Autofire, Limited Ammo 3*
- **Sap Mortar:** Damage 6, Crit 5, Range [Medium], Encumbrance 4, Price 180 acorns, *Blast 4, Immobilize 1, Limited Ammo 3, Indirect*
- **Fungal Spore Cannon:** Damage 5, Crit 6, Range [Medium], Encumbrance 3, Price 220 acorns, *Blast 5, Poison 2, Limited Ammo 2, Prepare 1*
- **Titan-Killer Harpoon:** Damage 12, Crit 3, Range [Short], Encumbrance 6, Price 600 acorns, *Pierce 5, Breach 2, Limited Ammo 1, Prepare 4, Vicious 2*
- **Deployable Spike Trap:** Damage 4, Crit 3, Range [Short], Encumbrance 3, Price 100 acorns, *Ensnare 3, Pierce 1, Prepare 2, Remains after deployment*

### Shields
Shields' defense values add to both Defensive (melee) and Deflection (ranged) defense values.
- **Acorn Cap Shield:** Defense +1, Encumbrance 2, Price 8 acorns,
- **Bark Shield:** Defense +2, Encumbrance 3, Price 25 acorns, *Defensive 1, Cumbersome 1*
- **Woven Branch Shield:** Defense +1, Encumbrance 2, Price 35 acorns, *Deflection 1*

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

## Armor

### Light Armor
- **Work Clothes:** Soak +1, Defense 0, Encumbrance 1, Price 20 acorns
- **Leather Vest:** Soak +1, Defense 1, Encumbrance 1, Price 45 acorns
- **Padded Jacket:** Soak +2, Defense 0, Encumbrance 2, Price 75 acorns
- **Courier Gear:** Soak +1, Defense 1, Encumbrance 1, Price 60 acorns, *Reduces falling damage by 1*

### Medium Armor
- **Scale Mail:** Soak +2, Defense 1, Encumbrance 2, Price 120 acorns, *Made from overlapping bark scales*
- **Reinforced Vest:** Soak +3, Defense 0, Encumbrance 3, Price 150 acorns
- **Guild Armor:** Soak +2, Defense 1, Encumbrance 2, Price 180 acorns, *Includes tool attachments - up to 2 encumbrance for tools is ignored*

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


# The Five Burrows - Detailed Guide

Each burrow has its own distinct character, challenges, and opportunities. Understanding the neighborhoods and notable locations helps bring The Great Burrow to life.

<div class='read'>

*From the observation deck atop the Whiskers Building, you can see it all. To the north, The Branchx sways in the morning breeze, rope bridges catching the light like spider silk. East, across the river, The Hives buzzes with activity as beetle-drawn carts haul the day's harvest. The scent of Lin's Brook's fish market carries on the wind, mixing with factory smoke. And there, barely visible through the morning haze, Scurry Island lurks—a shadow on the water where desperate creatures make desperate choices. Five burrows, five ways of life, one Great Burrow. The city spreads before you like a promise—or a threat.*

</div>

## Mousehattan - The Vertical Metropolis

Rising from a rocky outcropping where ancient oak roots penetrate stone, Mousehattan is the beating heart of commerce and ambition. Three massive oaks—the Trading Oak, the Council Oak, and the Old Growth—create a natural vertical city where fortunes are made and lost, where the old ways clash with new money in a never-ending dance of power and progress.

### Geography & Infrastructure

#### The Vertical City
- **The Rock**: A natural granite outcropping forms the backbone, chambers carved over generations
- **Root Highways**: Oak roots create natural "avenues" running through the stone
- **Seven Levels**: From the Sub-Basement tunnels to the Crown Level penthouses
- **Natural Springs**: Three underground springs with ancient water rights
- **The Great Underground Hub**: Central station connecting all five burrows

#### Transportation Systems
- **Vertical Shafts**: Rope and pulley systems between levels, operated by union crews
- **Root Runners**: Elite messenger mice who know every shortcut and hidden passage
- **Bark Slides**: Polished channels for rapid descent (climbing back up costs extra)
- **The Express**: Direct Underground service to other burrows for premium prices

\columnbreak

- **Private Lifts**: Wealthy families maintain personal vertical transport

### Districts

#### Wall Street (Financial District)
Literally carved into the main rock wall beneath the Trading Oak, this is the economic heart of The Great Burrow.
- **The Acorn Exchange Trading Floor**: Inside the Trading Oak's hollow, sets prices forest-wide
- **Root Vaults**: Ancient storage chambers where old families keep their wealth
- **Counting Rooms**: Traditional notched-stick tallying systems still in use
- **Grove Rights Office**: Where oak territory ownership is registered
- **Futures Pit**: Where next season's acorn prices are frantically negotiated
- **The Stone Steps**: Where bankrupt traders traditionally announce ruin

#### Times Squeak (Entertainment District)
Where five major tunnels converge beneath interlocking roots, buzzing with 24-hour activity.
- **Firefly Lantern District**: Managed colonies provide atmospheric lighting
- **The Squeak**: Famous performance venue for death theater and comedy
- **Roasted Seed Row**: Street vendors selling traditional and fusion snacks

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

- **The Moonlight Market**: After-hours trading in "fell off the tree" goods
- **Pleasure Dens**: Fermented root beer halls and honey lounges
- **The Never-Dark**: Underground plaza lit continuously by captive fireflies

#### Upper East Roots (Old Money Residential)
Carved into the most stable oak root systems, home to established families.
- **The Acorn Club**: Exclusive social organization requiring 5-generation membership
- **Gallery Row**: Displaying rare seeds, pressed leaves, and natural art
- **Private Warren Entrances**: Multi-generation family homes with dedicated access
- **The Four Hundred Hall**: Meeting place for descendants of original settlers
- **Root Gardens**: Private cultivation chambers for rare plants
- **The Grooming Parlors**: Where status is displayed through whisker styling

#### Midtown Tunnels (Commercial Center)
Busy shopping districts and merchant headquarters serving all creatures.
- **The Great Bazaar**: Indoor market spanning three levels
- **Craftsmouse Quarter**: Traditional trades, apprenticeship guilds
- **Honey Board**: Where Hives products are priced daily
- **Fur & Whisker**: Grooming and social networking center
- **The Goods Yards**: Warehouses storing commodities from all burrows
- **Messenger Central**: Where courier services compete for contracts

#### Village Burrows (Bohemian Quarter)
Maze-like informal tunnels housing artists, radicals, and newcomers.
- **The Crumb**: Famous intellectual gathering spot and debate hall
- **Underground Press Alley**: Bark-carved printing blocks, radical publications
- **Cheap Rent Warrens**: Most affordable housing, most "character"
- **The Gnaw**: 24-hour diner for night workers and bohemians
- **Radical Row**: Where union organizers and political activists meet
- **The Burrow Cooperative**: Experimental communal living arrangements

#### The Sub-Basements (Forgotten Depths)
Deep tunnels below official city levels, home to the desperate and the hidden.
- **The Forgotten Deeps**: Pre-city excavations, rumors of giant bones
- **Tunnel Rat Territory**: Where those who can't afford proper housing dwell
- **The Black Channels**: Smuggling routes known only to crime families
- **Old Mine Shafts**: Abandoned borings, now shelter for the desperate
- **The Bone Yards**: Where they say the first giants fell



### The Kaiju Creatures & City Defenses

#### The Giants That Walk
The creatures of Mousehattan live in constant awareness of the titans that could end everything with a single misstep.

- **Bears ("The Mountain That Moves")**: Full evacuations when one approaches. The Great Trampling of 20 years ago still shapes city planning.
- **Deer ("The Antlered Spirits")**: Can step over the East River in shallow spots. The Antler Scrape incident shut down the Trading Oak for weeks.
- **Moose ("The Darkness")**: Rare but most feared. Their movement literally reshapes landscapes.
- **Wild Boars ("Earth Shakers")**: Their rooting can collapse entire tunnel systems overnight.

#### Defense Systems
- **The Watch**: Elite scouts monitor giant movements, using coded bell signals
- **Deep Shelters**: Reinforced chambers in every district for "Titan Events"
- **The Bells of Mousehattan**: Five great bells that ring evacuation patterns
- **Offering Stations**: Strategic food piles to divert giants from populated areas
- **The Stillness Protocol**: When giants pass, absolute silence is law

<div class='note'>

#### <u>Mousehattan Sayings</u>

- "Every leaf has two sides" (opportunity and danger)
- "The oak remembers" (old debts are never forgotten)
- "Connected from root to crown" (having full protection)
- "The family provides" (mafia code)
- "Giants walk where they will" (acceptance of the uncontrollable)
- "Make your hole bigger" (rat entrepreneurial spirit)
- "Three acorns for luck" (traditional blessing)
- "Deep pockets, shallow roots" (new money insult)

</div>

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

### Demographics & Culture

#### Population Breakdown (Total: ~28,000)
- **40% Mice** (11,200): Old families, bankers, traditionalists
- **25% Rats** (7,000): Entrepreneurs, "connected" families, new money
- **15% Voles** (4,200): Middle management, service workers
- **10% Hamsters** (2,800): Merchants, storage specialists
- **5% Weasels** (1,400): Information brokers, fixers
- **3% Shrews** (840): Analysts, accountants, detail workers
- **2% Others** (560): Ferrets (dealmakers), visiting species


#### Social Stratification

**The Establishment (Old Money)**
- **The Four Hundred**: Direct descendants of the original oak-carvers
- **Acorn Nobility**: Families controlling prime harvest territories for generations
- **The Root Board**: Informal council of major family heads who set policy
- **Grove Rights Holders**: Ancient claims to specific oak territories

**The Connected (Crime Families)**
- **Made Creatures**: Full members of the major syndicates
- **Associates**: Working with but not sworn to families
- **The Respected**: Those who pay protection and stay quiet
- **The Watched**: Potential problems or informants

**The Strivers (Working Class)**
- **Union Members**: Protected by various trade organizations
- **Free Workers**: Unaffiliated, vulnerable to exploitation
- **The Climbers**: Young ambitious creatures from other burrows
- **Night Shift**: Those who work dangerous hours for better pay

### The Underground Economy

#### The Rat Syndicate
The dominant organized crime structure, built on old-country traditions and new-world ambition.

**Major Families:**
- **The Longtail Family**: Controls waterfront smuggling and dock unions. Run by Don Salvatore Longtail.
- **The Whisker Brotherhood**: Protection rackets and construction. Led by the Council of Three Brothers.
- **The Gray Coats**: Newest family challenging old territories. Young, aggressive, led by Lucia "The Shadow" Gray.

**Operations:**
- **"Insurance"**: Protection money from every business
- **The Numbers**: Illegal acorn lottery running daily
- **Seed Running**: Smuggling rare seeds between burrows
- **Union Control**: Influence over dock and construction workers
- **Loan Sharking**: Acorns at impossible interest rates

\columnbreak

#### The Weasel Network
A looser confederation specializing in information and flexibility.
- **The Flex**: Their ability to slip through anything, physically and socially
- **Information Brokerage**: "We know what you did last autumn"
- **Blackmail Rings**: Compromising information on establishment figures
- **Message "Delays"**: Courier services that read interesting mail
- **The Mediators**: Playing all sides in family conflicts

### Daily Life in Mousehattan

#### Work Culture
The city runs on rigid schedules tied to the Acorn Exchange bell.

- **The Dawn Bell**: Markets open, the city springs to life
- **Morning Climb**: Thousands ascending from deep warrens to work levels
- **Whisker Break**: Traditional mid-morning grooming and networking hour
- **The Closing Bell**: End of official trading, beginning of nightlife
- **The Night Shift**: When the real city emerges—dangerous but profitable

#### Food & Dining

**Traditional Establishments:**
- **Sal's Seedcake**: "Best in the city" (Whisker Brotherhood protected)
- **The Gnaw**: 24-hour diner for night shift workers
- **Mama's Nut House**: Classic vole-run family restaurant
- **The Acorn & Stem**: Upscale dining for business meetings

**Trendy Spots:**
- **Honey Lounges**: Expensive Hives imports, firefly ambiance
- **Fusion Holes**: Mixing cuisines from all five burrows
- **Root Beer Gardens**: Fermented sap served in carved acorn shells
- **Underground Supper Clubs**: Secret dining experiences

**Street Food:**
- Roasted seeds with exotic spices
- Fermented root beer from barrel carts
- Fresh sprout salads in leaf wraps
- Candied bark strips (sweet and savory)

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

#### Entertainment & Nightlife

**High Culture:**
- **The Metropolitan Nest**: Opera and classical performances
- **Gallery Row**: Seed sculptures and pressed flower art
- **The Acorn Club**: Where deals happen over aged root beer

**Popular Entertainment:**
- **Times Squeak Shows**: Theater, comedy, acrobatics
- **Bug Fights**: Controversial betting on insect battles
- **The Squeakeasy Chain**: Hidden bars throughout the city
- **Dance Burrows**: Where young creatures court and posture

**The Seedier Side:**
- **The Moonlight Market**: Anything for sale after dark
- **Gambling Dens**: From dice to racing beetles
- **Scent Parlors**: Exotic pheromone experiences
- **Fight Clubs**: Illegal but tolerated if discrete


### Notable Personalities

#### The Power Brokers
- **Victoria Silverpaw**: Matriarch of the oldest mouse banking family
- **Commissioner Bruno Tailslash**: Head of Burrow Security (quietly "connected")
- **Judge Cornelius Whiskerworth**: Incorruptible... mostly
- **Councilmouse Penelope Quicktail**: Reform candidate with dangerous ideas

#### The Connected
- **Don Salvatore Longtail**: Most powerful crime boss
- **Stella "The Shriek" Weaselton**: Information broker extraordinaire
- **Fat Tony Cheesewhisker**: Runs the biggest gambling operation
- **The Ferret Sisters**: Mysterious fixers who "solve problems"

#### The Operators
- **Maxine "Max" Scurry**: Best Root Runner in the city
- **Professor Algernon Nibbles**: Radical writer and troublemaker
- **Rosie Redtail**: Owns three honey lounges, knows everyone's secrets
- **Charlie "The Nose" Snifferton**: Can smell a bad deal from three tunnels away

### Adventure Hooks

#### Crime & Corruption
- **Family War**: The Gray Coats moving on Longtail territory
- **The Big Score**: Someone's planning to rob the Acorn Exchange
- **Witness Protection**: Protecting a rat who's ready to testify
- **Union Trouble**: Construction unions split between families
- **The Cleaner**: Someone's eliminating witnesses before a big trial

\columnbreak

#### Financial Intrigue
- **Market Manipulation**: Someone's cornering acorn futures
- **The Counterfeit Seeds**: Fake rare seeds flooding the market
- **Inheritance Dispute**: Old family fortune, multiple claimants
- **The Audit**: Investigating massive fraud at a major trading house
- **Hostile Takeover**: Crime family moving into legitimate business

#### Social Tensions
- **The Revolutionary**: Organizing workers against both families and establishment
- **Gentrification Wars**: Village Burrows residents fighting development
- **The Blackmail Ring**: Someone has dirt on half the Root Board
- **Species Tension**: Mice establishment vs. rat new money boiling over
- **The Underground Railroad**: Helping creatures escape crime family debts

#### Titan-Related Crises
- **The Prophet**: Titan-touched mouse claims to speak for the giants
- **Offering Theft**: Someone's stealing from giant-distraction food stores
- **The Shelter Scandal**: Deep Shelters sold to highest bidders only
- **Bear Sign**: Fresh markings suggest a den dangerously close
- **The Unbeliever**: Influential creature denying giant danger

#### Mystery & Investigation
- **The Missing Messenger**: Root Runner vanished with sensitive information
- **Museum Heist**: Priceless pre-city artifacts stolen
- **The Ghost**: Someone's impersonating a dead crime boss
- **Serial Killer**: Someone's hunting specific types of creatures
- **The Mole**: Crime family infiltrator in the government

<div class='example'>

##### A Day in Mousehattan
Dawn Bell rings at 6 AM sharp. Amelia Quickwhisker, junior analyst at Claw & Associates, begins her climb from Level 3 warren to the Midtown offices. She grabs fermented seeds from a cart, dodges a Root Runner, and checks the Acorn Exchange early numbers on the public boards.

At work, she notices unusual trading patterns—someone's buying up Lin's Brook shipping futures. During Whisker Break, she overhears two rats discussing "insurance" for her firm. The closing bell at 6 PM doesn't end her day; there's a client dinner at The Acorn & Stem.

Walking home through Times Squeak, she's careful to look confident but not wealthy. The Moonlight Market is setting up, and she recognizes a weasel from the Gray Coats watching her building. Tomorrow she'll take a different route. In Mousehattan, paranoia is just good sense.

</div>

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

### Relationships with Other Burrows

#### Economic Ties
- **The Branchx**: Source of construction labor and some muscle
- **The Hives**: Honey futures drive major market sector
- **Lin's Brook**: Shipping controlled by Longtail Family interests
- **Scurry Island**: Where deals happen that can't happen here

#### Criminal Networks
- **Protection Rackets**: Extending into Branchx construction
- **Smuggling Routes**: Through Lin's Brook docks to Scurry Island
- **Information Networks**: Weasels have creatures in every burrow
- **Money Laundering**: "Investments" in other burrow businesses

#### Cultural Exchange
- **Gentrification**: Mousehattan money changing other burrows
- **Brain Drain**: Ambitious creatures drawn to the vertical city
- **Cultural Appropriation**: Establishment mice adopting "quaint" customs
- **Underground Movements**: Revolutionary ideas spreading outward

<div class='note'>

#### <u>GM Tips for Mousehattan</u>

**Emphasize Vertical Space**
Remember creatures are constantly climbing up or down. Social status literally relates to elevation. Use vertical chase scenes and the constant threat of falling.

**Layer the Corruption**
Everyone's connected to someone. The honest cop has a cousin in the mob. The reformer takes campaign contributions from crime families. Nothing is simple.

**Giants as Weather**
Treat titan appearances like severe weather events. Regular creatures have evacuation plans, emergency supplies, and titan insurance. It's a fact of life that shapes everything.

**Old vs. New Money**
Play up tension between established mouse families and ambitious rat entrepreneurs. Use architecture to show this—ancient carved chambers vs. new flashy construction.

**The Code**
Whether criminal or establishment, everyone follows unwritten rules. Breaking these codes has consequences. Even heroes need to navigate these social expectations.

</div>

\columnbreak

### Unique Mousehattan Elements

#### The Acorn Economy
- Morning trading bells set the day's prices
- Futures markets for next season's harvest
- Complex derivatives based on weather patterns
- Underground markets in "pre-dropped" acorns
- Currency speculation between burrow economies

#### Vertical Transportation Rights
- Ancient elevator shaft claims passed through families
- Public vs. private lift access creating social friction
- Root Runner guilds controlling message routes
- Bootleg slides carved by criminal elements
- The politics of who maintains the ropes

#### Seasonal Challenges
- **Spring**: Flooding in lower levels from snow melt
- **Summer**: Heat in upper levels, titans most active
- **Autumn**: Harvest season chaos and market volatility
- **Winter**: Heating costs and hoarding accusations

This is Mousehattan: where ambition builds as high as the oaks, where everyone knows someone who knows someone, and where the bells that warn of giants also ring in each day's opportunities. In the vertical city, you're always climbing toward something—or falling from it.

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

# The Branchx - The Canopy Commons

High above the forest floor, where ancient oaks and maples create a natural metropolis of branches and hollows, The Branchx sprawls through the canopy like a three-dimensional maze of working-class pride and territorial ambition.

## Geography & Infrastructure

### The Vertical Territory
- **The Ancient Grove:** Fifty massive oaks and seventy grand maples form the core
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

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

## Demographics & Culture

### Population Breakdown *(Total: ~18,000)*
- **60% Squirrels (10,800):** Traditional majority, various subspecies
- **25% Chipmunks (4,500):** Essential courier class
- **10% Flying Squirrels (1,800):** Elite transport and message services
- **3% Mice (540):** Usually Mousehattan gentrifiers or climbers
- **2% Others (360):** Including reformed rats, adventurous voles

### Social Hierarchy - The Height System

#### Crown Touch Elite *(Levels 6-7)*
- **The Acorn Lords:** Control prime harvest territories passed through generations
- **Bridge Barons:** Families who built and maintain major crossing monopolies
- **The Old Nests:** Generational wealth measured in hollow ownership
- **Winter Cache Dynasties:** Those who never experience hunger season
- **Height Rights:** Legal documents proving branch ownership going back centuries

#### High Branch Comfortable *(Levels 4-5)*
- **Skilled Crafters:** Master builders, rope weavers, bridge engineers
- **Union Officers:** Those who've risen through the ranks to leadership
- **Established Merchants:** Running shops for generations
- **Professional Couriers:** Elite messengers with perfect safety records
- **Branch Managers:** Literally managing specific tree territories

#### Working Branches *(Levels 2-3)*
- **Construction Crews:** The backbone of Branchx identity
- **Apprentice Crafters:** Learning trades, hoping to rise
- **Day Laborers:** Taking whatever work is available
- **Night Shift Workers:** Higher pay for predator-risk hours
- **Maintenance Teams:** Keeping bridges and routes safe

#### Ground Scrape Struggling *(Level 1)*
- **New Arrivals:** Earning their first branch rights
- **The Nestless:** Sleeping in communal shelters or borrowed spaces
- **Failed Climbers:** Those who fell from higher status
- **Gang Prospects:** Young creatures seeing crime as only option
- **The Forgotten:** Elderly or injured with no family support

### The Families and Gangs

#### The Nutcracker Union - Power Through Solidarity

The most powerful organization in The Branchx, combining legitimate labor representation with less savory enforcement activities.

**Leadership Structure:**
- **Big Boss Hazelnut:** A scarred gray squirrel who rose from construction to control the union
- **The Council of Seven:** Representatives from major trades (construction, rope-making, bridge-building, etc.)
- **Shop Stewards:** On-site representatives who ensure compliance and collect dues
- **The Breakers:** Enforcement wing handling "difficult negotiations"

**Operations:**
- Controls all major construction hiring - no union card, no work
- "Insurance" services protecting job sites from "accidents"
- Pension fund management (with creative accounting)
- Strike organization and scab deterrence
- Political influence through campaign contributions

**Union Culture:**
- Morning shape-up at Union Tree determines day's work assignments
- Elaborate initiation rituals for new members
- Widows and orphans fund for those lost to work accidents
- "Coffee and acorns" meetings where real business happens
- The union card is more valuable than most creatures' life savings

#### The Tailwind Gang - Speed Above All

Chipmunk-dominated courier collective that's evolved into a powerful information network.

**Organization:**
- **Streak Swiftcheek:** Legendary racer turned gang leader
- **Route Bosses:** Control specific message paths and territories
- **Runners:** Young chipmunks proving themselves
- **The Weather Eyes:** Scouts who monitor conditions
- **The Memory Bank:** Elders who remember every route and shortcut

**Operations:**
- Message delivery monopoly on time-sensitive communications
- Information brokering - they read the mail
- Racing circuit with heavy betting
- Route protection from rival gangs
- Training academy for young runners

#### Corvid-Affiliated Groups - Serving Unknown Masters

**The Black Feathers:** Mysterious squirrels and other creatures who've made dark bargains
- Provide ground intelligence to crow networks
- Guaranteed protection from hawk attacks (mostly)
- Required to steal specific items crows designate
- Marked by small crow feather worn behind ear
- "Better to serve the clever than feed the hungry"

**Shiny Things Collective:** Thieves with corvid connections
- Steal items of no mammalian value but corvid interest
- Payment in protection and occasional warnings
- Never fully understand what crows want or why
- Complex drop-off rituals at designated "gift trees"

**The Murder's Paws:** Most feared gang in the canopy
- Direct enforcement arm of crow interests
- Led by "Blackbeak's Voice" - a squirrel who claims to speak for crows
- Territory includes prime branches near corvid roosts
- Even other gangs avoid confrontation with them
- Rumors of strange corvid magic and intelligence

#### Traditional Families - Old Branch Aristocracy

**The Oakheart Clan:** First Family of The Branchx
- Trace lineage to original canopy settlers
- Control three of the five Ancient Grove oaks
- Elaborate family tree (literally) carved into heartwood
- Bitter rivals with upstart Mapleseed Collective
- Matriarch Silviana Oakheart rules from Crown Touch mansion

**Swiftbranch Dynasty:** Flying squirrel elite
- Monopoly on night-time transport services
- Intermarried with Mousehattan banking families
- Private gliding academy for family members only
- Control the most profitable zip-line routes
- Young rebels increasingly joining gangs instead

**The Mapleseed Collective:** Progressive coalition
- Alliance of middle-branch families pushing reform
- Advocate for public branch ownership
- Run cooperative businesses and schools
- Led by Councilsquirrel Marcus Redtail
- Target of both union and traditional family harassment

\columnbreak

<div class='note'>

#### <u>Branchx Sayings</u>

- "High branch, warm winter" (elevation equals security)
- "Every bridge sways" (nothing is certain)
- "Nuts before glory" (practical priorities)
- "The hawk's shadow" (constant danger)
- "Branch born, sky sworn" (pride in canopy life)
- "Splinters build character" (hard work virtue)
- "A crow's promise" (something you can't trust)
- "Union strong, union long" (solidarity motto)
- "Check your knots twice" (always verify safety)
- "The fall remembers" (past failures haunt you)

</div>

## Daily Life & Economy

### Work Culture - The Rhythm of the Canopy

#### The Daily Cycle
- **Pre-Dawn Shape-Up (5 AM):** Workers gather at Union Tree for assignments
- **Dawn Patrol (5:30 AM):** Checking overnight storm damage and predator signs
- **Morning Shift (6 AM - 2 PM):** Prime working hours with maximum light
- **Whisker Break (10 AM):** Traditional work stoppage for grooming and gossip
- **Afternoon Shift (2 PM - 6 PM):** Second crews take over major projects
- **Sunset Scramble (6 PM):** Desperate race to safety as predators emerge
- **Night Shift (7 PM - 3 AM):** Dangerous work with double pay and death benefits

#### Seasonal Patterns
- **Spring:** Bridge repair season after winter damage
- **Summer:** Major construction projects while weather holds
- **Autumn:** Frantic acorn harvest requiring every available paw
- **Winter:** Indoor work - rope making, tool repair, planning

### Traditional Industries

#### Construction - The Pride of The Branchx
- **Nest Building:** From simple shelters to elaborate multi-family complexes
- **Bridge Engineering:** Secret techniques passed through apprenticeships
- **Hollow Expansion:** Carefully carving without killing trees
- **Platform Construction:** Work spaces suspended between branches
- **Emergency Reinforcement:** Storm-proofing and predator-proofing

**Construction Hierarchy:**
- Master Builders (10+ years experience)
- Journeycreatures (3-10 years)
- Apprentices (1-3 years)
- Helpers (entry level)
- Tool-carriers (children learning the trade)

#### Rope Making - The Binding Trade
- **Spider Silk Harvesting:** Dangerous negotiations with web-builders
- **Bark Fiber Processing:** Stripping, soaking, and weaving
- **Vine Cultivation:** Growing specific species for strength
- **Quality Testing:** Lives depend on rope integrity
- **Specialty Products:** From climbing lines to bridge cables

#### Acorn Economy - Seasonal Lifeblood

**Territory System:**
- Ancient rights to specific trees and branches
- Harvest licenses sold by controlling families
- Share-cropping arrangements for poorer creatures
- Territorial disputes settled by union or violence

**Processing Industry:**
- Fresh consumption vs. storage preparation
- 67 traditional preparation methods
- Fermentation for winter preservation
- Grinding for flour and meal
- Export preparation for other burrows

### Underground Economy

#### The Crow Market - Where Things "Fall"
- **Location:** Hidden platforms in the Crow Zones
- **Hours:** Dusk to midnight, corvid protection guaranteed
- **Goods:** Items of dubious origin, no questions asked
- **Currency:** Barter, favors, or corvid tokens
- **Protection:** Pay the crows or become prey

#### Protection Rackets - Safety for Sale
- **Hawk Insurance:** Pay for crow interference during attacks
- **Bridge Tolls:** "Maintenance fees" for safe crossing
- **Construction Site Security:** Preventing "accidents"
- **Night Shift Protection:** Escorts through dangerous hours
- **Territory Taxes:** Pay to work certain branches

#### Information Networks
- **Message Interception:** Couriers who read interesting mail
- **Gossip Markets:** Trading social intelligence
- **Height Papers:** Forged documents for social climbing
- **Union Cards:** Black market membership for non-citizens
- **Route Maps:** Secret paths sold to smugglers

<div class='example'>

##### A Day in the Life: Nutkin Firmgrip, Construction Worker

Nutkin wakes at 4:30 AM in his Level 2 family nest, shared with six relatives. Coffee—bitter bark tea—and yesterday's acorn cake before the climb to Union Tree. At shape-up, Boss Hazelnut assigns him to bridge repair on the dangerous Gap crossing. 

The crew takes the long route, avoiding Crow Zone territories where the Murder's Paws extracted "tolls" last week. Work is hard but steady—replacing rotted planks while watching for hawks. During Whisker Break, talk turns to the new Mousehattan development. "Taking our best branches," someone spits.

Lunch on the designated break-branch: shared seedcakes and gossip. Nutkin's cousin mentions the Tailwind Gang is recruiting. Better money, but dangerous work. The afternoon shift sees a close call—a hawk's shadow sends everyone scrambling for cover. Mitch Quicktail is too slow. The memorial fund will need contributions.

Sunset scramble is chaos—hundreds of workers racing darkness home. Nutkin makes it to his branch as the first owl hoots. Dinner is communal stew in the courtyard. His daughter shows him her climbing progress. His son talks about joining the union. 

Night brings exhausted sleep and dreams of higher branches. Tomorrow, if the weather holds and the hawks are hunting elsewhere, he'll do it all again. It's a hard life, but it's his life. Branch born, sky sworn.

</div>

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

## Notable Locations in The Branchx

### Historic Sites
- **The First Bridge:** Monument to canopy connection, still maintained but no longer used
- **Oldoak Hollow:** Where the burrow was founded, now a museum
- **The Memorial Wall:** Names of the hawk-taken, updated monthly
- **Union Tree:** Where labor first organized, still hosts morning shape-up
- **The Broken Branch:** Site of the Great Fall disaster 40 years ago

### Working Landmarks
- **The Nutcracker Hall:** Union headquarters, social center, and hiring hall
- **Central Crossing:** Busiest bridge intersection, five routes converge
- **The Tunnel Terminal:** Where underground dreams died, now storage
- **Shift-Change Square:** Where crews gather morning and evening
- **The Tool Library:** Communal equipment maintained by the union

### Social Venues
- **The Knothole:** Roughest bar in the canopy, union-protected
- **Acorn Cap:** Working-class social club, cheap drinks and solidarity
- **The Racing Branch:** Courier competition venue, heavy betting
- **Tail's End:** Where old squirrels tell stories over fermented sap
- **The Crow's Laugh:** Dangerous bar in the Crow Zones

### Hidden Spots
- **Crow's Nest Neutral:** Where deals get made under corvid protection
- **The Broken Tunnel:** Smuggler's highway beneath the canopy
- **Ghost Hollow:** Abandoned after hawk attack, said to be haunted
- **The Undergrowth:** Secret ground-level meeting spot for radicals
- **Cache Valley:** Hidden between branches, emergency food stores

## Notable Personalities

### Union Leadership
- **"Big Boss" Hazelnut Graysquirrel:** Union president, former construction worker with scars to prove it. Fair but ruthless when crossed. "The union is family, and family comes first."
- **Maple Quickpaw:** Secretary-Treasurer, knows where every acorn is buried. Rumored to have dirt on half the government.
- **Bruno "The Breaker" Heavytail:** Head of union enforcement. Missing an ear from a crow encounter. "Accidents happen to those who forget to pay dues."

### Gang Leaders
- **Streak Swiftcheek:** Tailwind Gang boss, still the fastest chipmunk in the canopy despite his age. Controls all major courier routes. "Information is speed, speed is power."
- **"Blackbeak's Voice":** Leader of the Murder's Paws, a gray squirrel who claims to speak for the crows. No one knows his real name. Even other gangs fear him.
- **Silky Darknose:** Runs the Shiny Things Collective. Female flying squirrel with connections throughout the underworld. "The crows want what they want."

### Traditional Powers
- **Matriarch Silviana Oakheart:** Rules the oldest squirrel clan from her Crown Touch mansion. 80 years old and sharp as a hawk's talon. "Height is in the blood, child."
- **Lord Reginald Swiftbranch III:** Flying squirrel aristocrat who controls night transport. Educated in Mousehattan but came home to rule. "We glide above your petty conflicts."
- **Councilsquirrel Marcus Redtail:** Leader of the progressive Mapleseed Collective. Pushing for public branch ownership. "The canopy belongs to all who work it."

### Street-Level Heroes
- **Nutkin Firmgrip:** Respected construction foreman who looks out for his crew. Lost his brother to a hawk, raises his nephew. "Check your knots twice, live to check tomorrow."
- **Chatter Speedwhisker:** Young chipmunk courier who knows every shortcut. Feeds information to both sides for survival. "I just deliver messages, don't write them."
- **Old Tom Scarbranch:** Retired bridge builder who runs a shelter for the nestless. Union pension keeps him comfortable. "Every creature deserves a warm branch."

### The Dangerous
- **Slash Redclaw:** Psychotic enforcer for the Murder's Paws. Takes payment in pain. "The crows like screaming."
- **The Ferret:** Information broker who somehow operates in The Branchx despite the species prejudice. No one knows where she nests. "Everything has a price, especially secrets."
- **Thistle Sharptooth:** Rogue union breaker who hires out to whoever pays. Survived three assassination attempts. "Solidarity is just another word for target."

\columnbreak

## Cultural Details & Traditions

### The Height Hierarchy in Practice
The vertical nature of Branchx society creates constant reminders of status:
- **Branch Etiquette:** Lower branch creatures must yield right-of-way
- **Vertical Addresses:** Nest locations include height designations
- **Climbing Permits:** Official documents required for accessing higher levels
- **Social Climbing:** Literal term for improving one's position
- **The Fall:** Social disgrace literally described as "falling to Ground Scrape"

### Crow Relations - A Complex Dance
The relationship between mammals and corvids remains mysterious and unsettling:
- **The Tribute Trees:** Specific locations where offerings are left for crows
- **Crow Tongue:** Mammals who claim to understand corvid speech (usually mad)
- **Protection Zones:** Areas where crow alliance guarantees safety from hawks
- **The Black Market:** Literally named for crow-controlled trade
- **Corvid Court:** When crows judge mammalian disputes (rare but binding)

### Union Culture & Working Pride
- **The Morning Whistle:** Traditional call to work, blown from Union Tree
- **Tool Blessing:** Ritual before dangerous jobs, "May your grip stay true"
- **The Widow's Share:** Portion of every job goes to support bereaved families
- **Apprentice Hazing:** Elaborate pranks that build solidarity
- **The Password:** Secret union phrases change weekly

### Seasonal Celebrations
- **First Leaf Festival:** Spring celebration of survival and new growth
- **The Harvest Dance:** Autumn acorn celebration, branch-shaking competitions
- **Bridge Day:** Honors builders and commemorates those lost to falls
- **The Night of Tails:** Midwinter festival where creatures show off grooming
- **Crow's Peace:** One night per year when corvids guarantee no attacks

<div class='note'>

#### <u>More Branchx Cultural Elements</u>

**Food Specialties:**
- Fermented acorn mash (working creature's drink)
- Bark-strip jerky for quick energy
- Seed-cake rolls sold at shift change
- "Crow's Gift" (mysterious berries that appear after tributes)

**Music & Entertainment:**
- Branch drumming communication/music
- Tail acrobatics competitions
- Death-defying bridge racing
- Work songs that coordinate construction
- Whisker theater (improvised comedy)

**Superstitions:**
- Crossed branches bring bad luck
- Never build on a branch where someone fell
- Owl pellets under the nest prevent night attacks
- A crow feather in your nest means you're marked
- White squirrels are either blessed or cursed

</div>

## Adventure Hooks

### Working-Class Drama
- **Strike Breaking:** Mousehattan money hiring scabs for new development, union planning violent response
- **The Fallen Brother:** Young squirrel must choose between family in union and lover in the gangs
- **Bridge Collapse Mystery:** Investigation reveals corruption in construction contracts
- **The Gentrification War:** Old families losing branch rights to wealthy newcomers
- **Pension Fund Theft:** Someone's embezzling from the union, retirees are desperate

### Canopy Noir
- **The Missing Courier:** Chipmunk vanishes with evidence of crow conspiracy
- **Protection Racket War:** Black Feathers vs. Murder's Paws for territory control
- **High Branch Murder:** Socialite pushed or fell? Everyone has motives
- **The Tunnel Body:** Corpse in abandoned section opens old wounds
- **Blackmail Branch:** Someone's photographing prominent creatures in compromising positions

### Survival Horror
- **New Hawk Tactics:** Predator learning to counter traditional defenses
- **The Crow Demands:** Corvids want something impossible, threaten to withdraw protection
- **Storm Season:** Multi-day tempest traps creatures without supplies
- **The Ground Surge:** Predators driving prey up from below
- **Night Terror:** Something's hunting that isn't an owl

### Political Intrigue
- **Union Election:** Corruption, violence, and Mousehattan interference
- **The Branch Rebellion:** Young creatures reject height hierarchy violently
- **Cross-Species Alliance:** Secret marriage between squirrel nobility and chipmunk courier
- **The Acorn Cartel:** Families conspiring to corner harvest market
- **Revolutionary Cells:** Ground Scrape organizing against entire system

### The Corvid Mystery
- **The Speaking Squirrel:** Someone claims true communication with crows
- **The Great Gathering:** All corvids leaving creates panic and opportunity
- **Shiny Thing Syndrome:** Crows demanding specific item no one understands
- **The Black Wing Prophecy:** Ancient warning about corvid intentions surfacing
- **Feather Fever:** Crow-gifted feathers granting strange abilities

## Relationships with Other Burrows

### With Mousehattan
- **Love/Hate Dynamic:** Need their money, resent their attitude
- **Labor Export:** Many squirrels commute for construction contracts
- **Gentrification Pressure:** Wealthy mice buying up prime branches
- **Cultural Clash:** "Soft-pawed acorn counters" vs. "primitive branch-swingers"
- **Underground Connections:** Direct service, but delayed "for maintenance"

### With Lin's Brook
- **Working-Class Solidarity:** Natural allies in labor struggles
- **Trade Competition:** Both bid for major construction projects
- **Union Cooperation:** Share organizing strategies and strike support
- **Cultural Exchange:** Intermarriage common between communities
- **Mutual Respect:** "Water workers understand honest labor"

### With The Hives
- **Trade Partners:** Honey for construction materials
- **Neutral Ground:** Neither threatens the other's interests
- **Skill Recognition:** Respect for different but equal expertise
- **Limited Mixing:** Some marriage connections, mostly professional
- **Stereotype:** "Ground dwellers, but hardworking ones"

### With Scurry Island
- **Criminal Pipeline:** Where troublemakers flee to disappear
- **Black Market:** Illegal goods flow both directions
- **Shared Resentment:** Both looked down upon by Mousehattan
- **Escape Route:** Underground railroad for creatures in trouble
- **Dark Reputation:** "Even they got out—what's your excuse?"

## GM Tips for The Branchx

<div class='note'>

#### <u>Running The Branchx</u>

**Emphasize Verticality**
Every scene should reinforce the three-dimensional nature of the canopy. Describe movements as climbs, leaps, and scrambles. Use height differences to show social status.

**Constant Predator Pressure**
The hawk's shadow should appear regularly. Make players paranoid about open sky. Use weather to increase or decrease threat levels.

**Union Politics**
The Nutcracker Union touches everything. Even non-labor stories should acknowledge their influence. They're both protectors and oppressors.

**Corvid Ambiguity**
Never fully explain crow motivations. They're alien intelligences with incomprehensible goals. Protection comes with costs no one understands.

**Class Consciousness**
Working-class pride battles economic anxiety. Characters should feel tension between solidarity and personal advancement.

</div>

### Unique Branchx Elements

#### The Construction Culture
- **Tool Worship:** Personal tools passed through generations with names and histories
- **Site Superstitions:** Elaborate rituals before starting new projects
- **The Measure:** Traditional building standards based on squirrel body lengths
- **Wood Whispering:** Master builders who "hear" what the tree wants
- **Failure Shame:** Collapsed structures haunt builders forever

#### The Courier Networks
- **Route Secrecy:** Paths passed from master to apprentice only
- **Speed Trials:** Monthly races determine route assignments
- **Weather Readers:** Specialists who predict flying conditions
- **The Memory Run:** Couriers who memorize messages, never write
- **Blood Bonds:** Courier partnerships sealed with ritual

#### The Height Economy
- **Branch Futures:** Speculation on which trees will grow tallest
- **Vertical Taxes:** Higher branches pay more but get better services
- **Lift Cartels:** Control of vertical transport creates fortunes
- **The Fall Insurance:** Policies covering social and literal dropping
- **Nest Flipping:** Buying low branches, improving, selling high

#### Survival Adaptations
- **Hawk Drills:** Every kit knows seventeen different alarm calls
- **Camouflage Fashion:** Clothing designed to blend with bark
- **The Scatter:** Choreographed escape patterns for groups
- **Dummy Nests:** Decoys to confuse predators
- **Silent Running:** Moving through branches without sound

This is The Branchx: where height determines worth, where every creature lives one shadow from death, where working-class pride built a vertical city reaching for the sky while keeping roots in tradition. Where bridges connect more than trees—they connect communities fighting to survive in a canopy that changes faster than a squirrel can climb. Where "earning your perch" means more than finding a branch—it means defending your right to exist in the only home your family has ever known.

In The Branchx, you're always climbing toward something—or falling from it. The question is: will you rise by lifting others, or by stepping on their backs? Either way, check your knots twice, watch the sky, and remember—every branch sways, but the union stands strong.

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

# The Hives - The Crossroads Community

Sprawling across the meadow clearings where forest meets grassland, The Hives earned its name from the dense, interconnected burrow complexes that honeycomb the rolling hills. This is The Great Burrow's most diverse community, where prairie dogs from the southern grasslands live next to mountain marmots, where traditional rabbit warrens neighbor innovative guinea pig terraces, and where the scent of a dozen different cuisines mingles in the evening air.

"Everyone finds their place in the swarm" isn't just a saying here—it's a way of life. In The Hives, success comes not through ancient bloodlines or crime family connections, but through hard work, community spirit, and the endless creativity that emerges when different cultures collide and cooperate.

## Geography & Infrastructure

### The Crossroads Location
The Hives occupies the strategic position where forest meets grassland, creating natural convergence points for trade and migration. Rolling hills provide defensive positions while meadow clearings offer space for markets and gatherings.

- **Gateway Hills:** Rolling terrain that naturally funnels trade routes from the southern grasslands
- **The Convergence:** Where multiple streams meet, creating natural stopping points for caravans
- **Meadow Flats:** Open areas perfect for markets, festivals, and temporary camps
- **Burrow Heights:** Terraced hillsides packed with multi-family housing complexes
- **The Commons:** Central gathering spaces shared by multiple neighborhoods

### Transportation Hub
As The Great Burrow's logistics capital, The Hives processes goods from across the known world. The burrow's prosperity depends on maintaining these vital trade connections.

- **Caravan Grounds:** Staging areas where external traders set up temporary camps, complete with rest houses, repair shops, and supply stores
- **The Great Interchange:** Where three Underground lines converge in a massive station handling 35,000+ daily passengers
- **Wagon Ways:** Wide paths designed for heavy freight from distant communities, maintained by cooperative work crews
- **The Sorting Yards:** Warehouse district where goods are processed, sorted, and distributed to all five burrows
- **Border Crossings:** Informal checkpoints where Rangers verify incoming traders and check for contraband

\columnbreak

### Mixed Infrastructure
The Hives showcases how different species' building traditions can combine to create something new and functional.

- **Insect Partners:** Beetles for heavy hauling, ants for micro-delivery, fireflies for lighting, all working in carefully negotiated partnerships
- **Traditional Warrens:** Multi-generational rabbit tunnel systems with sophisticated ventilation
- **Terrace Communities:** Guinea pig-style hillside housing adapted by other species
- **Workshop Districts:** Small manufacturing and repair facilities often sharing tools and expertise
- **Cultural Centers:** Community buildings serving different immigrant populations

### Districts

#### Central Commons *(The Heart)*
The beating heart of The Hives, where all communities converge. The Great Interchange dominates the underground levels while markets and meeting spaces fill the surface.

- The Great Interchange Underground station with multi-lingual signage
- Multi-cultural markets open from dawn to midnight
- Community meeting halls designed for different species' needs
- The Diversity Council chambers with translation services
- Tourist information and cultural orientation centers

#### Meadow Heights *(Established Families)*
The oldest district, where traditional rabbit families maintain their ancestral warrens and honey operations.

- Traditional rabbit warrens with honey production facilities
- Multi-generational family compounds with private gardens
- The old Hive Registry and historical society
- Premium residential areas with established property rights
- Conservative community leadership resisting rapid change

#### Grassland Quarter *(Prairie Immigrants)*
A piece of the southern plains transplanted to the forest, where prairie dog communities maintain their democratic traditions.

- Prairie dog settlements with distinctive circular architecture
- Wide, communal burrow systems designed for group living
- Grain processing and storage facilities using traditional methods
- Community kitchens where meals are shared events
- Democratic town-hall style governance with regular votes

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

#### Mountain Slopes *(Highland Immigrants)*
Where marmot families from the high country have recreated their alpine communities with adapted techniques.

- Marmot settlements built into hillsides with natural drainage
- Stone-working and mineral processing workshops
- Terraced gardens using mountain water management techniques
- Seasonal celebration grounds for solstice festivals
- Craft workshops specializing in mountain techniques

#### Innovation District *(Mixed Community)*
The newest and most experimental district where young families from different species create fusion communities.

- Guinea pig agricultural experiments with vertical farming
- Cross-cultural fusion workshops teaching combined techniques
- Young families from multiple species living as neighbors
- Experimental housing cooperatives with shared facilities
- The Integration Center for newcomers learning city ways

#### The Yards *(Industrial Zone)*
The engine of The Hives' economy, processing goods from across the region.

- Warehouses storing everything from pine nuts to seaweed
- Beetle-powered manufacturing using sustainable practices
- Repair shops fixing caravan wagons and trade goods
- Transportation company headquarters coordinating shipments
- Worker housing and union halls organizing fair labor

#### Night Market *(Entertainment District)*
When the sun sets, this district comes alive with music, food, and celebration.

- After-hours dining featuring fusion cuisine experiments
- Cultural performance venues showcasing homeland traditions
- Firefly-lit evening markets selling exotic goods
- Mixed-species social clubs breaking down barriers
- The artistic community hub fostering creative collaboration

#### Border Camps *(Temporary Housing)*
The ever-changing edges where new arrivals first experience The Hives.

- Seasonal worker accommodations during harvest times
- New arrival processing centers with basic services
- Caravan support services for traveling merchants
- Emergency housing during predator alerts or floods
- Ranger coordination facilities monitoring approaches

\columnbreak

## Demographics & Culture

### Population Breakdown *(Total: ~24,000)*
The Hives' strength lies in its diversity, with no single species holding overwhelming majority.

- **20% Rabbits** (4,800): Established families controlling traditional honey operations and old warren properties
- **18% Prairie Dogs** (4,320): Grassland immigrants bringing democratic traditions and grain expertise
- **15% Voles & Field Mice** (3,600): Working class backbone in service and logistics industries
- **12% Guinea Pigs** (2,880): Recent immigrants revolutionizing agriculture with terracing innovations
- **10% Marmots** (2,400): Mountain folk bringing stone-craft and weather wisdom
- **8% Hamsters** (1,920): Merchant families specializing in storage and inventory management
- **7% Hedgehogs** (1,680): Night shift specialists in entertainment and security
- **5% Shrews** (1,200): Technical experts managing insect partnerships
- **5% Mixed/Other** (1,200): Dozens of species in smaller numbers

### Cultural Dynamics

#### The Established Community
The original inhabitants struggle to maintain their traditions while adapting to change.

- **Old Warren Families:** Rabbit dynasties tracing lineage to The Hives' founding, controlling prime honey territories
- **The Founding Principles:** Original cooperative values emphasizing mutual aid over individual profit
- **Cultural Preservation:** Maintaining forest traditions while selectively adopting innovations
- **Economic Stability:** Established businesses and property ownership creating generational wealth

#### The Grassland Wave
Prairie dog communities brought new ideas about governance and community organization.

- **Prairie Dog Collectives:** Democratic decision-making through regular assemblies and consensus building
- **Grain Culture:** Diversifying beyond honey with sophisticated grain storage and processing
- **Social Innovation:** New forms of community cooperation like shared child-rearing
- **Integration Challenges:** Adapting open-plains culture to enclosed forest life

<div class='note'>

#### <u>Hives Sayings</u>

- "Every creature finds their place in the swarm" (everyone belongs somewhere)
- "Many burrows, one community" (unity in diversity)
- "The hive remembers all its workers" (honoring everyone's contributions)
- "Sweet as cooperation" (highest compliment for working together)
- "Busy as the Crossroads" (constantly active and productive)
- "Different flowers, same garden" (diversity creating beauty)

</div>

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

#### The Mountain Communities
Marmot families from the high country bring specialized skills and alpine wisdom.

- **Marmot Crafters:** Master stone-workers creating lasting infrastructure from local materials
- **Alpine Traditions:** Seasonal festivals tied to mountain weather patterns and celestial events
- **Water Management:** Advanced terracing and irrigation techniques preventing erosion
- **Weather Wisdom:** Generations of knowledge predicting seasonal changes

#### The New Generation
Young creatures born in The Hives create fusion cultures their parents never imagined.

- **Cross-Cultural Families:** Inter-species relationships producing new family structures
- **Innovation Pioneers:** Combining traditions to solve problems in unexpected ways
- **Urban Adaptation:** Forest-born creatures fully embracing city life and opportunities
- **Cultural Bridge-Builders:** Translating between communities and mediating conflicts

## Economy

### Primary Industries
The Hives' economy thrives on diversity and interconnection.

- **Logistics & Distribution (30%):** Processing goods from external trade, managing warehouse districts, coordinating shipments
- **Small Manufacturing (25%):** Textiles combining multiple traditions, fusion crafts, household goods
- **Agriculture & Food (20%):** Honey production, grain processing, fusion cuisine restaurants
- **Services (15%):** Shops catering to diverse tastes, repair services, cultural businesses
- **Transportation (10%):** Caravan support, Underground operations, courier networks

### The Trade Hub
The Hives' position makes it the natural gateway for external commerce.

- **External Goods Processing:** Sorting, grading, and repackaging for urban markets
- **Caravan Services:** Rest houses, wagon repair, supply provisioning, guide services
- **Currency Exchange:** Converting between acorn standard and regional trade goods
- **Information Brokerage:** News from distant communities commands premium prices
- **Seasonal Markets:** Major trading festivals during spring arrivals and autumn departures

### Manufacturing Diversity
Small workshops demonstrate the power of cultural fusion.

- **Textile Fusion:** Prairie dog weaving meets rabbit fur processing meets guinea pig dyeing
- **Food Processing:** Preserving techniques from multiple traditions extend shelf life
- **Craft Workshops:** Marmot stone-carving tools modified for beaver woodworking
- **Repair Services:** Fixing everything from mountain gear to grassland wagons
- **Custom Work:** Specialized items for different species' anatomical needs

\columnbreak

### Cultural Economy
The Hives' diversity creates unique economic opportunities.

- **Restaurants:** From traditional warren cooking to grassland barbecue to fusion experiments
- **Entertainment:** Music halls where prairie dog drums meet rabbit flutes
- **Education:** Language schools, cultural orientation, inter-species etiquette classes
- **Arts & Crafts:** Traditional expressions and shocking fusion pieces
- **Tourism:** "Authentic diversity experiences" draw visitors from homogeneous burrows

## Daily Life

### Community Rhythms
Life in The Hives follows patterns that accommodate multiple species' needs.

- **Dawn Markets:** Fresh goods arrive via Underground, early traders get best selection
- **Morning Commute:** Thousands heading to other burrows for work pack the Interchange
- **Midday Convergence:** Peak activity as caravans arrive and markets buzz
- **Afternoon Workshops:** Manufacturing and craft production in full swing
- **Evening Gatherings:** Community meals in public spaces, cultural events beginning
- **Night Markets:** Entertainment district comes alive with music and exotic foods

### Cultural Fusion in Practice

#### Language Mixing
The Hives has developed its own dialect combining words from multiple languages. A typical conversation might include prairie dog technical terms, rabbit formal address, guinea pig musical intonations, and marmot weather words.

<div class='example'>

##### A Day in the Crossroads Market

"*Buenos días*, Grandfather Chen! Your *terraza* vegetables look *geschmack* today!"

"*Ahoy* there, young Pip! Try these *nouvelle* carrot-grain cakes - my daughter's *fusion création*!"

"*Wunderbar*! Hey, *amigo*, you hear about the *kerfuffle* at the Interchange? Some *haute monde* mouse from Mousehattan made *ein gross faux pas* about prairie dog housing!"

"*Ay, Dios mío*! These city folk need to learn - *hier* in The Hives, we respect *alle* creatures!"

</div>

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

#### Fusion Cuisine
The Hives' restaurants showcase culinary innovation born from cultural collision.

- **Honey-Glazed Grain Balls:** Rabbit sweetness meets prairie dog staples
- **Mountain Berry Salsa:** Marmot preserves with guinea pig spices
- **Five-Culture Stew:** Each community contributes one ingredient
- **Fusion Bakeries:** Combining baking traditions produces unique breads
- **Street Food Innovation:** Portable foods adapted for multiple species

#### Hybrid Celebrations
Festivals blend traditions creating entirely new celebrations.

- **Convergence Festival:** Annual celebration where each community showcases culture
- **Harvest Harmony:** Combining autumn traditions from grassland and forest
- **New Year Fusion:** Multiple calendar systems create week-long celebration
- **Unity Feast:** Monthly communal meals in each district
- **Children's Day:** Young creatures learn about all cultures through play

### Housing Diversity
Architecture reflects the community's varied needs and traditions.

- **Traditional Warrens:** Rabbit-style multi-generational complexes with modern amenities
- **Prairie Compounds:** Open communal spaces with minimal privacy but maximum community
- **Mountain Terraces:** Hillside construction using marmot engineering principles
- **Innovation Cooperatives:** Experimental housing mixing all architectural styles
- **Temporary Accommodations:** Flexible spaces for seasonal workers and new arrivals

### Work Culture
The Hives' cooperative spirit extends to the workplace.

- **Cooperative Pride:** Success measured by benefit to community, not individual wealth
- **Skills Sharing:** Regular workshops where creatures teach their specialties
- **Flexible Arrangements:** Accommodating different species' schedules and needs
- **Union Organization:** Worker solidarity crosses species lines in pursuit of fairness
- **Entrepreneurship:** Small businesses supported by community micro-loans

## Notable Locations

### Community Centers
- **The Great Hall:** Multi-purpose space hosting everything from weddings to political debates, designed to accommodate creatures of all sizes
- **Cultural Quarter:** Separate buildings for prairie dog assemblies, rabbit warren councils, marmot stone circles
- **The Integration Center:** One-stop shop for new arrivals - housing assistance, language classes, job placement
- **Community Kitchens:** Shared cooking facilities where fusion cuisine is born
- **The Forum:** Open-air democratic meeting space modeled on prairie dog traditions

\columnbreak

### Economic Hubs
- **The Exchange:** Central marketplace where anything can be bought, sold, or traded
- **Caravan Square:** Dusty plaza where external traders conduct business and share news
- **Workshop Row:** Concentration of small manufacturers sharing tools and expertise
- **The Sorting Yards:** Massive warehouse complex processing regional trade
- **Union Hall:** Headquarters for United Workers Alliance, crossing species lines

### Cultural Venues
- **The Harmony Theater:** Performance space with rotating stages for different cultural needs
- **Festival Grounds:** Open meadow reserved for celebrations and large gatherings
- **The Gallery Walk:** Artist studios and exhibition spaces showcasing fusion art
- **Music Gardens:** Outdoor venues designed with natural acoustics
- **The Story Circle:** Traditional gathering space where elders share cultural histories

### Traditional Sites
Despite rapid growth, The Hives preserves its historical roots.

- **The First Hive:** Original honey operation turned into working museum
- **Warren Prime:** Ancestral rabbit tunnels with memorial plaques
- **The Cooperation Stone:** Monument where species first agreed to share the land
- **Elder Grove:** Sacred trees where community ceremonies occur

<div class='note'>

#### <u>The Great Interchange</u>

The Underground station serves as The Hives' beating heart. Three levels accommodate different traffic:

**Upper Level:** Local shuttles to nearby districts
**Middle Level:** Express services to other burrows  
**Lower Level:** Freight and cargo operations

During rush hour, specialized "pushers" help pack commuters into overcrowded cars while multilingual announcements attempt to maintain order. The station's famous Food Court offers cuisine from every corner of The Hives, making it a destination in itself.

</div>

## Governance & Politics

### The Diversity Council
The Hives pioneered inclusive governance accommodating multiple decision-making traditions.

**Structure:**
- **Community Representatives:** Each major ethnic group sends delegates
- **Rotating Leadership:** Council chair position rotates between communities monthly
- **Translation Services:** Ensuring all voices are literally understood
- **Consensus Requirements:** Major decisions need 75% agreement
- **Veto Powers:** Any community can block actions affecting them directly

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

**Functions:**
- **Resource Allocation:** Distributing public funds fairly between districts
- **Cultural Mediation:** Resolving conflicts between different traditions
- **External Relations:** Coordinating with other burrows and trade partners
- **Emergency Response:** Managing crises requiring community-wide action
- **Development Planning:** Balancing growth with community character

### Community Organizations
Grassroots groups provide the real governance in daily life.

- **Neighborhood Associations:** Hyperlocal governance for specific blocks
- **Cultural Societies:** Preserving homeland traditions while adapting to city life
- **Worker Cooperatives:** Democratic ownership of businesses and workshops
- **Youth Councils:** Giving voice to the fusion generation
- **Elder Circles:** Wisdom keepers advising on traditional matters

### Political Movements
The Hives' diversity creates a complex political landscape.

- **The Integrationists:** Promoting cultural fusion and shared identity
- **The Preservationists:** Maintaining distinct cultural boundaries
- **The Progressives:** Embracing change and experimentation
- **The Cooperatives:** Expanding democratic economics
- **The Regionalists:** Strengthening ties with homeland communities

## Urban Tensions & Challenges

### The Honeycomb Family: Agricultural Mafia
Not all of The Hives' prosperity comes from honest work. The Honeycomb Family evolved from traditional beekeeping dynasties into a sophisticated criminal organization.

#### Operations & Influence
- **Honey Trade Control:** Manipulating prices through "quality certification" requirements
- **Caravan "Insurance":** Protection services that create the threats they guard against
- **Market Stall "Permits":** Unofficial fees for prime selling locations
- **Labor "Mediation":** Resolving disputes in ways that benefit family interests
- **Political Influence:** Subtle corruption maintaining the cooperative facade

#### Methods & Philosophy
Unlike Mousehattan's violent syndicates, the Honeycomb Family operates through economic pressure and social manipulation.

- **Agricultural Traditions:** Using farmer respectability as cover for crime
- **Community Integration:** Family members serve on councils and charity boards
- **Soft Power:** Preferring bankruptcy to bloodshed
- **Protection Services:** Actually providing security while extracting tribute
- **Information Networks:** Knowing everyone's business through "friendly concern"

\columnbreak

### Infrastructure Crisis

#### The Great Interchange Breakdown
The massive transportation hub is failing under pressure no one anticipated during construction.

**Physical Problems:**
- **Platform Overcrowding:** Dangerous crushes during rush hours
- **Tunnel Degradation:** Water seepage weakening support structures
- **Signal Failures:** Outdated systems causing regular delays
- **Ventilation Issues:** Air quality declining in deeper levels

**Political Problems:**
- **Funding Disputes:** Burrows arguing over who pays for repairs
- **Mole Engineer Strikes:** Demanding hazard pay for dangerous conditions
- **Maintenance Corruption:** Repair funds disappearing into connected paws

#### Housing Shortage
Rapid population growth has overwhelmed The Hives' inclusive housing policies.

- **Overcrowded Warrens:** Designed for 4 creatures housing 12
- **Tent Cities:** "Temporary" camps becoming permanent slums
- **Rising Rents:** Established families profiting from newcomer desperation
- **Speculation:** Mousehattan investors buying properties sight unseen
- **Cultural Displacement:** Traditional neighborhoods losing character to gentrification

### Social Tensions

#### Integration vs. Preservation
The fundamental question of The Hives: How much change is too much?

- **Language Conflicts:** Which dialect to use in schools and official business
- **Cultural Appropriation:** Fusion going too far, disrespecting traditions
- **Religious Differences:** Sacred practices clashing with secular governance
- **Educational Disputes:** What history to teach the fusion generation
- **Festival Conflicts:** Limited public space causing scheduling battles

#### Economic Inequality
Despite cooperative ideals, wealth gaps are widening.

- **Established vs. Newcomer:** Old families controlling prime resources
- **Skills Premium:** Technical workers earning multiples of laborers
- **Property Concentration:** Land rights inherited, not earned
- **Capital Access:** New businesses can't compete with established ones
- **Generational Mobility:** Young creatures seeing no path to prosperity

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

### Environmental & Security Challenges

#### Predator Vulnerability
The Hives' open meadow location makes it the most exposed burrow to aerial threats.

- **Hawk Hunting Grounds:** Open spaces provide perfect attack approaches
- **Limited Cover:** Few trees or structures for quick shelter
- **Surface Dependencies:** Many activities require above-ground exposure
- **Evacuation Challenges:** Diverse population has different mobility needs
- **Border Length:** Extensive perimeter impossible to fully monitor

#### Seasonal Extremes
Weather hits The Hives harder than the forest-sheltered burrows.

- **Spring Flooding:** Meadow streams overflow into lower districts
- **Summer Droughts:** Water shortages affecting dense population
- **Autumn Fires:** Dry grass creates serious risks
- **Winter Exposure:** Less natural insulation than forested areas
- **Climate Unpredictability:** Traditional weather wisdom failing

### The Beetle Uprising
The Hives' economy depends on insect partnerships, but the relationship is fraying.

#### Growing Tensions
- **Overwork:** Beetles pushed beyond sustainable limits
- **Pheromone Resistance:** Some insects developing immunity to control scents
- **Organization:** Beetles beginning to coordinate across handlers
- **Sabotage:** "Accidents" increasing in frequency
- **Demands:** Shorter hours, better food, breeding rights

#### Economic Impact
- **Shipping Delays:** Packages arriving late or not at all
- **Manufacturing Slowdowns:** Beetle-powered equipment failing
- **Agricultural Crisis:** Honey production dropping without beetle assistance
- **Public Services:** Waste management and construction suffering
- **Black Market:** Illegal pheromones and beetle-trading emerging

## Opportunities Amid Challenges

### Innovation Through Adversity
The Hives' diversity becomes its greatest strength during crises.

- **Cross-Cultural Solutions:** Each tradition contributing unique approaches
- **Rapid Adaptation:** Diverse communities pivoting quickly to new realities
- **Mutual Aid Networks:** Different groups supporting each other
- **Creative Economics:** New business models emerging from necessity
- **Social Innovation:** Pioneering inclusive governance structures

### Competitive Advantages
- **Cultural Diversity:** Multiple perspectives preventing blind spots
- **Trade Hub Status:** Central location ensuring economic relevance
- **Community Spirit:** Cooperative traditions building resilience
- **Adaptability:** Constant change making flexibility normal
- **External Relationships:** Strong connections with homeland communities

\columnbreak

## Notable NPCs

### The Power Brokers

#### Councilrabbit Honeycomb
**Elder Mother Beatrice Honeyclover**
- Leader of both legitimate honey business and criminal enterprise
- Grandmother persona hiding ruthless intelligence
- "Sweet as cooperation" while controlling the sugar supply
- Genuinely believes crime provides community stability

#### Councilpig Whistlebelly
**Professor Gustavo Terrazamor**
- Agricultural innovator and integration advocate
- Speaks five languages with musical guinea pig accent
- Pioneered vertical farming in abandoned tunnels
- Building cross-species progressive coalition

#### Chief Mediator Brownfur
**Marcus "Peace-Maker" Brownfur** (Prairie Dog)
- Diversity Council's primary conflict resolver
- Famous for talking down species riots
- Maintains neutral stance despite pressure
- Secret romantic relationship crossing enemy communities

### The Connected

#### Little Honey
**Salvatore "Sally Honey" Mellifera** (Rabbit)
- Honeycomb Family's chief enforcer
- Appears as bumbling sweet-seller
- Controls market stall "permits"
- Never been seen to commit violence personally

#### The Beetle Whisperer
**Thrix-ka** (Shrew)
- Only creature who truly understands beetles
- Negotiating between insects and mammals
- Rumored to be organizing beetle unions
- May be planning something bigger

### The Operators

#### Mama Terrace
**Elena Cascada-Morales** (Guinea Pig)
- Runs three restaurants and informal banking
- Helps new immigrants navigate the system
- Information broker with ethics
- Knows everyone's grandmother

#### The Festival King
**Chester "Party Time" Brightstripe** (Chipmunk)
- Organizes cultural celebrations
- Somehow profits from free events
- Connected to every community
- May be Intelligence Service asset

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

### The Innovators

#### The Fusion Chef
**Marie-Cloudette Whiskerling** (Field Mouse)
- Created honey-grain-beetle fusion cuisine
- Restaurant is neutral ground for all factions
- Uses food to bridge cultural divides
- Hiding escaped creatures in secret basement

#### Young Terrace
**Miguel "Mikey T" Terrazamor** (Guinea Pig)
- Councilpig Whistlebelly's rebellious son
- Running underground fusion music clubs
- Dating outside his species and class
- Building youth movement across communities

## Adventure Hooks

### Cultural Conflicts
- **Festival Sabotage:** Someone's trying to ruin Convergence Festival, destroying community unity
- **The Translation Crisis:** Universal translator beetles suddenly refuse to work, chaos ensues
- **Sacred Ground:** Development threatening multiple communities' religious sites
- **Culture War:** Extremists pushing for species separation gain momentum

### Economic Mysteries  
- **The Honey Heist:** Someone's replacing real honey with synthetic, economy in freefall
- **Warehouse Wars:** Goods disappearing between arrival and distribution
- **Counterfeit Goods:** Fake products destroying The Hives' reputation
- **The Grain Conspiracy:** Prairie dog merchants being systematically ruined

### Political Intrigue
- **Council Corruption:** Evidence emerges of vote-buying in Diversity Council
- **The Succession Crisis:** Honeycomb Family matriarch dying, war brewing
- **External Influence:** Mousehattan trying to economically colonize The Hives
- **Democratic Breakdown:** Consensus system failing, violence threatening

### Infrastructure Disasters
- **The Great Collapse:** Interchange tunnel system failing, thousands trapped
- **Beetle Strike:** Insects refuse to work, economy grinding to halt
- **Water Wars:** Drought pitting communities against each other
- **The Tent City Fire:** Disaster in temporary housing threatens thousands

### Community Challenges
- **The Integration Test:** High-profile inter-species marriage causing riots
- **Youth Exodus:** Entire generation leaving for other burrows
- **The Plague:** Disease spreading through overcrowded housing
- **Cultural Preservation:** Last speakers of homeland languages dying

\columnbreak

### Predator Crises
- **Hawk Season:** Aerial predators discovering the exposed market squares
- **The Titan Passage:** Giant deer migration path shifting through The Hives
- **Underground Predator:** Something hunting in the deep tunnels
- **The Swarm:** Predatory wasps establishing hive near border

## The Future of The Hives

### Emerging Trends
- **Cultural Synthesis:** New shared identity emerging from fusion
- **Economic Innovation:** Cooperative models spreading to other burrows
- **Political Evolution:** Direct democracy experiments expanding
- **Regional Leadership:** Becoming model for inclusive communities

### Challenges Ahead
- **Sustainable Growth:** Managing expansion without losing character
- **Cultural Balance:** Preserving diversity while building unity
- **Economic Justice:** Ensuring prosperity reaches all communities
- **External Pressure:** Resisting exploitation by wealthier burrows

### Potential Futures

#### The Melting Pot Path
Full integration creating new hybrid culture, loss of distinct traditions but stronger unified identity.

#### The Mosaic Path  
Maintaining separate communities within shared framework, risking fragmentation but preserving diversity.

#### The Innovation Path
Becoming the creative capital through cultural fusion, risking commercialization of traditions.

#### The Breakdown Path
Tensions exploding into conflict, communities retreating into ethnic enclaves, cooperative dream dying.

<div class='example'>

##### Running Adventures in The Hives

The Hives works best for stories about community, identity, and cooperation. Focus on:

- **Cultural misunderstandings** creating conflict
- **Economic pressures** testing community bonds  
- **Infrastructure** as both problem and solution
- **Diversity** as strength and challenge
- **Innovation** born from fusion

Let players navigate between communities, building bridges or watching them burn.

</div>

This is The Hives: where the forest meets the grasslands, where ancient traditions meet innovative solutions, and where creatures from across the region come together to build something greater than the sum of their parts. A community that proves diversity is strength, cooperation is prosperity, and that home is not where you come from, but where you choose to build your life alongside others who share your dreams.

<div class="footnote">THE GREAT BURROW<BR />
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

#### <u>Running Titan-Caused Disasters</u>

When titans threaten Lin's Brook:
1. **Warning Phase**: Perception checks to notice signs
2. **Evacuation Phase**: Leadership/Athletics to organize escape
3. **Crisis Phase**: Survival checks, rescue opportunities
4. **Aftermath**: Rebuilding creates new conflicts

Make titans feel like natural disasters, not monsters to fight. Focus on community response and heroic rescues.

</div>

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

<div class="footnote">THE GREAT BURROW<BR />
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

#### Historic Sites
- **The First Dam:** Now a monument and museum
- **Founders' Lodge:** Where the original builders lived
- **The Great Slipway:** Where major construction is launched
- **Old Fish Market:** Traditional morning gathering place

#### Working Waterfront
- **Shellcracker's Dock:** Otter-run, busiest ferry terminal
- **The Lumber Yards:** Beaver-controlled, strictly organized
- **Mill Row:** Water-powered workshops, dawn to dusk noise
- **The Net Lofts:** Where fishing gear is made and mended

#### Cultural Venues
- **The Waterlogged:** Dockworker tavern, otter-dominated
- **Slide Stadium:** Professional racing venue
- **The Current:** Underground music venue in old mill
- **Greenbank Gallery:** Former warehouse, now contentious art space

#### Hidden Spots
- **The Sunken Lodge:** Underwater meeting place for shady deals
- **Smuggler's Inlet:** Hidden cove for moving contraband
- **The Deep Pools:** Where the biggest fish hide
- **Forgotten Spillway:** Abandoned dam, now black market hub

## Water-Based Industries & Transportation

### The Fishing Fleet
Lin's Brook feeds The Great Burrow through its massive fishing operations. Pre-dawn launches see hundreds of bark boats and log rafts heading out, each crew knowing their territory by ancestral right. The catch determines daily prices across all burrows - a poor fishing day means hungry bellies and economic ripples.

- **Boat Types:** From single-otter kayaks to multi-family beaver barges
- **Territory System:** Enforced by tradition and occasional violence
- **Processing:** Shore-side cleaning stations operate round the clock
- **Distribution:** Fast couriers rush fresh fish to other burrows

### Construction & Engineering
The beavers of Lin's Brook literally built The Great Burrow. Their expertise in water management, structural engineering, and sustainable harvesting makes them indispensable. Every major project needs Lin's Brook workers.

- **The Builders Guild:** Controls all major construction contracts
- **Apprentice System:** Seven-year training from kit to master
- **Innovation vs. Tradition:** Young engineers clash with old masters
- **Export Teams:** Travel to other burrows for specialized projects

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

### Water Transportation Networks
The waterways are Lin's Brook's highways. Complex systems of canals, locks, and seasonal routes connect the burrow to the wider world. Control of these routes means power.

- **Ferry Services:** Otter-dominated, fiercely competitive
- **Cargo Hauling:** Beaver freight companies move bulk goods
- **The Lock Masters:** Control flow and charge passage fees
- **Smuggling Routes:** Underwater paths known only to locals

## Social Dynamics & Community Life

### Otter-Beaver Relations
The two dominant species maintain an uneasy partnership. Beavers build and maintain; otters fish and transport. When they work together, Lin's Brook thrives. When they clash, the entire waterfront suffers.

<div class='note'>

#### <u>Playing Social Tensions</u>

Lin's Brook tensions are about pride and tradition:
- **Work Ethics:** Beavers value persistence, otters value speed
- **Territory:** Water rights disputes go back generations
- **Intermarriage:** Creates both bridges and complications
- **Young vs. Old:** Traditional ways challenged by new ideas

Use these tensions for roleplay, not combat. A beaver-otter argument over construction methods can reveal character and advance plot without violence.

</div>

### Guild Politics & Labor Pride
Lin's Brook runs on guild power. The Builders Guild, Dockworkers Union, and Fishercreatures Cooperative wield more influence than any politician. Guild membership determines social standing, marriage prospects, and economic survival.

#### The Builders Guild
- **Membership:** Primarily beaver, some muskrats, rare others
- **Ranks:** Apprentice, Journeycreature, Master, Grandmaster
- **Politics:** Conservative leadership resists new techniques
- **Power:** Can shut down construction across Great Burrow

#### Dockworkers Union
- **Membership:** Otter-dominated but increasingly diverse
- **Organization:** Crew-based with elected representatives
- **Tactics:** Strategic strikes at peak shipping times
- **Connections:** Some crews have crime family ties

\columnbreak

#### Fishercreatures Cooperative
- **Structure:** Democratic profit-sharing collective
- **Membership:** Open to all who fish, regardless of species
- **Issues:** Territory disputes and quota arguments
- **Innovation:** Younger members push sustainable practices

### Working-Class Culture
Lin's Brook creatures take pride in physical work. Calloused paws are badges of honor. Office workers from Mousehattan are viewed with suspicion - "soft-paws" who don't understand real labor.

#### Values & Traditions
- **Dawn Work:** "The creek rewards early risers"
- **Tool Care:** Well-maintained tools reflect character
- **Apprenticeship:** Learning from masters, not books
- **Community First:** Neighbors help with lodge-raising
- **Honest Labor:** Better poor and proud than rich and soft

#### The Gentrification Crisis
Greenbank's spread threatens traditional Lin's Brook culture. Artisanal shops replace tool stores. Craft breweries push out worker taverns. Weekend tourists photograph "authentic" working creatures like zoo exhibits.

- **Rising Rents:** Working families forced to Downstream
- **Cultural Tourism:** "Experience real dock life!"
- **Boutique Products:** $50 acorn "hand-smoked" fish
- **Resistance:** Vandalism and boycotts increasing

## Notable Personalities

### The Old Guard
- **Master Builder Cornelius Flatail:** Grandmaster of Builders Guild, opposes all change
- **Captain Marina Shellcracker:** Runs largest ferry service, knows every current
- **"Iron Paw" Brutus:** Dockworker boss with crime connections
- **Grandmother Willow:** Eldest otter, remembers the Great Washing

### The Rising Tide
- **Cascade Swiftcurrent:** Young otter advocating for sustainable fishing
- **Engineer Brooke Innovative:** Beaver proposing radical dam improvements
- **Union Rep Rocky Muskrat:** Fighting for multi-species dock crews
- **Chef Lillypad:** Frog immigrant revolutionizing fish cuisine

### The Connected
- **Sal "The Salmon" Silverscale:** Runs north dock protection
- **The Downstream Boys:** Gang controlling salvage rights
- **Madame Current:** Information broker working from houseboat
- **Riptide Smugglers:** Use underwater routes for contraband

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

## Challenges & Threats

### Environmental Pressures
Lin's Brook faces mounting ecological challenges that threaten its survival. The water that gives life also brings danger.

#### Water Quality Crisis
- **Upstream Pollution:** Runoff from distant settlements
- **The Hives' Pesticides:** Beetle farming chemicals in water
- **Algae Blooms:** Warm summers create dead zones
- **Fish Die-Offs:** Increasingly common, cause unknown

#### Climate Disruption
- **Irregular Flooding:** Traditional patterns failing
- **Drought Cycles:** Low water threatens mill power
- **Ice Jam Disasters:** Winter thaws cause catastrophic floods
- **Species Migration:** New fish species disrupting ecosystem

### Infrastructure Decay
The Great Dam and its supporting infrastructure are aging. Maintenance costs soar while funding shrinks. Political fights over repairs threaten the entire system.

- **The Great Dam:** Needs complete rebuild within five years
- **Secondary Dams:** Three near failure, patches insufficient
- **Underground Flooding:** Subway tunnels regularly submerged
- **Bridge Network:** Storm damage faster than repairs

### Giant Interactions
Water attracts giants. Lin's Brook's position along Whisker Creek makes it particularly vulnerable to titan disruptions.

#### Moose Crossings
Summer brings moose wading through the creek. A single crossing can destroy weeks of construction, kill dozens, and traumatize survivors. The burrow maintains:
- **Spotting Network:** Upstream watchers with horn signals
- **Evacuation Routes:** Practice drills save lives
- **Sacrificial Structures:** Built to break and absorb impact
- **Counseling Circles:** For survivors of moose events

#### Bear Season
Salmon runs attract bears. The entire burrow sometimes evacuates for days. Economic disruption is massive, but fighting bears means certain death.
- **The Bear Bell:** Ancient warning system
- **High Caches:** Food stored above bear reach
- **Tribute Piles:** Fish left to distract bears
- **Prayer Circles:** Asking spirits for bear-free seasons

\columnbreak

<div class='example'>

##### Surviving a Moose Crossing

The morning started like any other at Shellcracker's Dock. Marina was checking ferry schedules when the upstream horns sounded - three long blasts. Moose.

"MOOSE! MOOSE! EVERYBODY TO HIGH GROUND!"

Workers dropped tools and ran for the evacuation slides. Marina stayed to untie the boats - lose the fleet and families starve. The ground shook as the giant approached.

The first wave hit as the moose's hoof entered the creek. Marina dove, grabbed a kit who'd frozen in terror, and swam hard for the safe pools. Behind them, the dock exploded into splinters.

Later, cleaning mud from her fur, Marina surveyed the damage. Three dead, seven missing, dock destroyed. But the boats survived. Tomorrow they'd rebuild. That's what Lin's Brook did.

</div>

## Adventure Hooks

### Working Waterfront Drama
- **Strike Breaking:** PCs hired to protect scab workers or support union
- **The Fixed Race:** Investigating slide-racing corruption
- **Inheritance Dispute:** Ancient water rights create family war
- **The New Technique:** Revolutionary building method divides guild

### Environmental Mysteries  
- **The Dying Creek:** Tracing source of upstream poison
- **Fish Whispers:** Strange behavior suggests something in deep water
- **The Missing Spawning:** Salmon don't return, economy crashes
- **Dam Rot:** Mysterious disease eating wooden structures

### Crime & Corruption
- **Protection War:** Two families claim same territory
- **The Sunken Treasure:** Rumors of riches in deep pools
- **Smuggling Ring:** Using guild connections for contraband
- **The Informant:** Someone's feeding info to authorities

### Giant Encounters
- **The Early Warning:** Upstream station goes silent
- **Bear Cult:** Some creatures worship the titans
- **The Sacrifice:** Someone's luring giants to destroy rivals
- **Giant Beaver:** Sightings of legendary protector

### Social Conflicts
- **Gentrification Riot:** Violence erupts in Greenbank
- **Species Integration:** Push for non-traditional guild members
- **The Whistleblower:** Exposing guild corruption from inside
- **Culture Wars:** Traditional festival becomes battleground

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

### Community Challenges
- **The Flood Fund:** Money for repairs has vanished
- **Evacuation Drill Disaster:** Practice becomes real emergency
- **The Tourist Invasion:** Weekend visitors disrupt crucial work
- **Youth Exodus:** Young creatures leaving for easier lives

## Relationships with Other Burrows

### Economic Connections
Lin's Brook's position as infrastructure hub creates complex relationships with other burrows. They build everyone's homes but often feel underappreciated.

#### With Mousehattan
- **Construction Contracts:** Major source of employment
- **Resentment:** "We build their towers, they look down on us"
- **Commuter Workers:** Daily migration for construction jobs
- **Gentrification Source:** Mousehattan money changing Greenbank

#### With The Branchx
- **Working Brotherhood:** Shared union organizing
- **Competitive Bidding:** Both burrows want construction contracts  
- **Cultural Exchange:** Similar working-class values
- **Joint Strikes:** Coordination threatens entire city

#### With The Hives
- **Food Trade:** Fish for honey, mutual dependency
- **Environmental Tensions:** Pesticide runoff concerns
- **Immigrant Workers:** Bees and others seeking dock work
- **Cultural Respect:** Both value hard work and community

#### With Scurry Island
- **Smuggling Networks:** Underwater routes connect them
- **Criminal Cooperation:** Families work together
- **Exile Destination:** Banished creatures flee there
- **Black Market Hub:** Stolen goods flow both ways

### Cultural Perceptions
How Lin's Brook sees others:
- **Mousehattan:** Soft-pawed parasites living off others' work
- **The Branchx:** Brothers in labor, allies in struggle
- **The Hives:** Hardworking but too trusting
- **Scurry Island:** Rough but honest about it

How others see Lin's Brook:
- **Mousehattan:** Necessary but crude, smell like fish
- **The Branchx:** Reliable allies with similar values
- **The Hives:** Skilled but clannish, resist change
- **Scurry Island:** Useful partners, dangerous enemies

\columnbreak

<div class='note'>

#### <u>GM Tips for Lin's Brook</u>

**Water Is Everything**
Make water central to every scene. The tide schedule determines when creatures work, eat, and sleep. High tide brings opportunities; low tide reveals secrets.

**Working Class Pride**
These creatures built the city with their own paws. They're not looking for pity - they want respect. Heroes earn trust through sweat, not speeches.

**Tradition vs. Progress**
Every advancement threatens someone's way of life. The old beaver who's built dams for 40 years sees new techniques as personal attacks. Play up generational conflicts.

**Giants as Weather**
Treat titan encounters like natural disasters. Focus on community response, not combat. Heroes save lives and minimize damage - they don't fight moose.

**Crime Is Practical**
Lin's Brook crime is about survival and territory, not elaborate schemes. Protection rackets, smuggling, and gambling feel natural in a working waterfront.

**Environmental Stakes**
Water quality affects everyone. A poisoned creek means no fish, no power, no life. Environmental threats can drive entire campaigns.

**Guild Power**
Guilds are more powerful than government here. Cross a guild and you can't work, can't eat, can't live in Lin's Brook. Use guild politics for social challenges.

</div>

### The Future of Lin's Brook

The working waterfront stands at a crossroads. Traditional ways clash with modern needs. The water that built the burrow now threatens it. Young creatures dream of easier lives while elders fear losing their identity.

Will Lin's Brook remain the strong back that carries The Great Burrow? Or will gentrification, environmental collapse, and social change sweep away generations of tradition like a giant's wake?

The tide is turning - the question is which way it will flow.

This is Lin's Brook: where water meets wood, where tradition meets change, where every creature knows that honest work and strong dams are all that stand between civilization and the flood. In the working waterfront, you earn your place with calloused paws and a willingness to rebuild when the giants come through.

<div class="footnote">THE GREAT BURROW<BR />
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

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

## Scurry Island - The Forgotten Burrow

<div class='read'>

*The morning mist parts to reveal Scurry Island across the choppy straits. Even from the mainland shore, you can see the Rangers on patrol atop the Heights, their scarred forms silhouetted against the dawn. Below them, smoke rises from the Harbor Market where anything—absolutely anything—can be bought for the right price. The broken ferry lists at the dock while desperate creatures argue over passage. This is the edge of civilization, where the forgotten come to disappear and the brave stand against the darkness. Here, survival isn't just a skill—it's the only currency that truly matters.*

</div>

Built on and around "The Old Giant," a massive fallen oak in the central clearing, Scurry Island exists as The Great Burrow's most dangerous paradox: simultaneously its most vital defense and most forgotten community. Ten thousand creatures scratch out existence on rocky shores and in dense interior woods, creating a society where mainland law holds no sway and only the strong—or clever—survive. The island serves as both haven for the desperate and fortress against the titans that would devour the city.

### The Ranger Paradox

The Rangers represent everything noble and terrible about Scurry Island. These elite scouts and fighters stand as the only organized defense against bears, moose, deer, and other giants that threaten The Great Burrow. Yet they recruit from the desperate, train through brutality, and die in numbers that would shock comfortable mainlanders.

<div class='note'>

#### <u>Understanding Titan Scale</u>

To small mammals, "titans" or "giants" are normal forest predators and large herbivores:
- **Bears**: Moving mountains of death
- **Deer/Moose**: Crushing hooves, accidental devastation
- **Hawks/Owls**: Aerial death (though corvids handle most)
- **Foxes/Coyotes**: Ground-level apocalypse
- **Humans**: Mythical world-enders (if they existed)

</div>

#### Ranger Organization

**Command Structure:**
- **Watch Commander Grimjaw**: One-eyed badger who earned rank through survival
- **Scout Wing**: Flying squirrels and bats for reconnaissance
- **Strike Teams**: Mixed-species heavy combat units
- **Trap Brigade**: Engineers of giant deterrence
- **The Blessed**: Veterans who've survived direct titan encounters

**Recruitment and Training:**
- Six-week program with 40% washout rate
- Live-fire exercises using captured predators
- The Oath: "Between the city and the dark"
- Specialized training by species strengths
- Final test: solo patrol in titan territory

**Equipment Arsenal:**
- **Poison Quills**: Porcupine needles with paralytic coating
- **Flash Powder**: Blinding charges for giant eyes
- **Scent Bombs**: Chemical deterrents and lures
- **Tangle Lines**: Root-fiber cables for tripping
- **The Black Darts**: Last resort killing tools

### Geography & Infrastructure

#### The Island Itself

Scurry Island's isolation shapes everything about its culture. The island stretches roughly two miles long and one mile wide, separated from the mainland by straits that vary from a quarter-mile to a full mile depending on tides. These waters, while navigable, create a psychological and practical barrier that keeps the island perpetually apart.

**Natural Features:**
- **The Heights**: Rocky northern plateau housing Ranger Command
- **Harbor Bay**: Natural southern inlet where ferries dock
- **The Fallen Giant**: Massive oak corpse serving as central landmark
- **Interior Woods**: Dense cover for fugitives and operations
- **Tidal Flats**: Eastern shallows exposing temporary land bridges
- **Western Cliffs**: Sheer drops facing the Deep Woods

**Infrastructure Challenges:**
- **Ferry System**: Three boats in theory, one functional in practice
- **No Bridge**: Proposals always die in mainland councils
- **Fresh Water**: Rain collection and rationed ferry deliveries
- **Power**: Stolen electric lines and generator black market
- **Communication**: Unreliable radio to mainland

\columnbreak

### Districts in Detail

#### Ferry Landing - Gateway to Shadows

The first thing newcomers notice is the smell: salt, rot, fear, and opportunity mixed into something uniquely Scurry Island. The Ferry Landing sprawls chaotically from the dock, with temporary structures rebuilt after each storm.

**Key Locations:**
- **The Last Stop Tavern**: Where Rangers drink and recruit
- **Customs House**: Abandoned building now hosting black market
- **The Greeter's Stand**: Where guides offer "protection"
- **Quick Paw Clinic**: No-questions medical care
- **The Board**: Job postings, missing creatures, bounties

**Culture**: Every creature at the Landing is either coming or going. Permanent residents know to spot the desperate (easy marks), the dangerous (avoid or ally), and the dying (Rangers past saving). The ferry schedule—when boats actually run—determines the rhythm of life.

#### Old Town - Where Tradition Survives

Built into ancient oak groves on the island's stable high ground, Old Town maintains the closest thing to respectability on Scurry Island. Original opossum and raccoon families control these warrens through tradition and subtle violence.

**Notable Features:**
- **The Death Theaters**: Opossum traditional performance spaces
- **Root Market**: Night bazaar in the tangled trees
- **Sanctuary Square**: Neutral ground enforced by all
- **The Old Families' Halls**: Warren complexes centuries old
- **Memory Gardens**: Where island history is preserved

**Old Town Customs:**
- "Playing dead" as formal greeting
- Sanctuary peace enforced with extreme prejudice
- Night business conducted by tail-light
- Family name means more than mainland law
- Children kept away from "mainland corruption"

#### Harbor Market - Anything for a Price

The commercial heart of shadow economy, Harbor Market never truly sleeps. Sprawling from the docks through temporary stalls and permanent shops, this is where the island's reputation is earned.

**Market Sections:**
- **The Clean Quarter**: Legitimate goods at mainland prices
- **Gray Alley**: Items of questionable provenance
- **The Black Rows**: Openly illegal merchandise
- **Flesh Market**: Not what mainlanders think—exotic foods
- **Information Row**: Secrets bought and sold

**What's for Sale:**
- Forged identity documents (10-50 acorns)
- Concentrated fermented sap (5 acorns per vial)
- Mainland contraband (double standard price)
- Ranger surplus equipment (buyer beware)
- Maps to titan territory (accuracy not guaranteed)
- Protection services (rates vary by threat)

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

#### The Lowland Shanties - Bottom of the Bottom

When everywhere else is full, when you can't afford even Old Town's cheapest warren, when the last ferry left without you—welcome to the Lowlands. Built on flood-prone ground, these ramshackle communities wash away with depressing regularity.

**Survival Strategies:**
- Build cheap, rebuild often
- Everything valuable stays portable
- Community watches for flood signs
- Higher ground = higher status
- Storm shelters shared by necessity

**Lowland Culture:**
- "One storm from homeless" mentality
- Fierce loyalty among the desperate
- Day labor at dawn by the docks
- Scavenging as primary economy
- Dreams of mainland escape

#### Ranger Heights - Fortress of the Brave

The island's highest ground hosts the Ranger Station, a complex of fortified buildings, training grounds, and memorials. From here, Rangers can see clear to the Deep Woods—and the threats emerging from them.

**Ranger Complex Features:**
- **Command Tower**: Watch Commander's strategic center
- **Training Grounds**: Where recruits learn or wash out
- **The Armory**: Weapons locked tighter than mainland banks
- **Trophy Hall**: Proof of kills and victories
- **Medical Ward**: Where the lucky wounded recover
- **The Wall of the Fallen**: Names carved in heartwood
- **Signal Towers**: Communication with mainland forces

**Daily Ranger Life:**
- Dawn training regardless of weather
- Equipment maintenance as meditation
- Patrol assignments by veterancy
- Evening debrief and intelligence sharing
- Night watches rotating constantly

#### The Warrens - What Happens in the Deep

Beneath Scurry Island lies a network of tunnels whose full extent no single creature knows. Started as storm shelters, expanded by smugglers, connected by fugitives, the Warrens now serve every illegal purpose imaginable.

**Warren Zones:**
- **The Fighting Pits**: Brutal entertainment for betting
- **Smuggler's Rest**: Hidden warehouse complexes
- **The Deep Dark**: Where creatures disappear permanently
- **Emergency Network**: Storm shelters and titan refuges
- **The Underneath Market**: When even Harbor Market won't sell it

**Warren Law:**
- What happens in the deep stays in the deep
- No mainland enforcement ever
- Disputes settled by combat or council
- Routes change to prevent mapping
- Emergency shelters open to all during disasters

### Demographics & Culture

#### Population Breakdown *(Total: ~10,000)*

**Established Residents (6,000):**
- **30% Opossums (3,000)**: Traditional families and survivors
- **25% Raccoons (2,500)**: Running most shadow businesses
- **10% Ferrets/Weasels (1,000)**: Information and smuggling
- **10% Mixed Species (1,000)**: Long-term fugitives and operators

**Temporary Residents (4,000):**
- **15% Active Rangers (1,500)**: Serving their terms
- **5% Retired Rangers (500)**: Too broken to leave
- **5% Recent Fugitives (500)**: Fleeing mainland justice
- **10% Transients (1,000)**: Seasonal workers and drifters

#### The Survival Hierarchy

Unlike mainland burrows with complex social structures, Scurry Island operates on brutal simplicity: those who survive longest make the rules.

**The Trunk Council:**
- **Mother Pale**: Ancient opossum, keeper of sanctuary law
- **Big Scar**: Raccoon controlling major smuggling
- **Watch Commander Grimjaw**: Ranger military authority
- **The Ferryman**: Whoever currently controls boat access
- **The Deepest**: Unknown figure controlling the Warrens

**Social Standing Markers:**
- Scars (especially from titans) = respect
- Sanctuary passes = connected
- Old Town address = established family
- Ranger insignia = temporary authority
- Warren access = dangerous player

\columnbreak

### The Shadow Economy

Scurry Island's economy operates on different principles than the mainland. Here, everything has a price, but that price might not be in acorns.

#### Black Market Operations

**Major Commodities:**
- **Information**: Who's looking for whom, what Rangers know, mainland secrets
- **Documents**: Forged papers, false identities, clean histories
- **Contraband**: Banned substances, stolen goods, forbidden items
- **Services**: Assassination, disappearance, protection, silence
- **Weapons**: From Ranger surplus to improvised explosives

**Price Examples:**
- New identity package: 50-200 acorns
- Mainland smuggling run: 20-100 acorns
- Concentrated sap (1 vial): 5 acorns
- Protection (1 week): 10-50 acorns
- Information (varies): 1-1000 acorns
- Making problems vanish: Negotiable

#### Legitimate Business

Even Scurry Island needs some legitimate economy:

**Ranger Economy:**
- Titan bounties from burrow coalition
- Trophy preparation and trade
- Equipment maintenance and supply
- Medical services for wounded
- Training services for private groups

**Service Industries:**
- Ferry maintenance (when running)
- Construction after storms
- Food service and taverns
- Temporary shelter rentals
- Guide services for newcomers

**Resource Extraction:**
- Salvage from titan encounters
- Driftwood and storm debris
- Specialized island plants
- Information brokerage
- Survival skill training

### Daily Life on the Edge

#### A Day on Scurry Island

**Dawn (6 AM):**
- Ferry horn announces first crossing (if running)
- Rangers change watch on the Heights
- Day laborers gather at the docks
- Night market winds down in Old Town
- Storm damage assessment begins

**Morning (9 AM):**
- Harbor Market reaches peak activity
- Ranger patrols deploy to mainland
- Construction crews repair storm damage
- Information brokers open for business
- The desperate seek day work

**Midday (12 PM):**
- Ferry attempts second crossing
- Training exercises at Ranger Heights
- Peak heat drives business underground
- Sanctuary hours begin in Old Town
- Fighters rest for evening bouts

**Afternoon (3 PM):**
- Black market shifts to gray goods
- Rangers return from patrol (if lucky)
- Storm preparations if weather threatens
- The Warrens begin to stir
- Smuggling operations plan night runs

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

**Evening (6 PM):**
- Final ferry crossing attempted
- Night market opens in Old Town
- Fighting pits begin taking bets
- Ranger memorial hour for the fallen
- Shadow economy fully awakens

**Night (9 PM):**
- The island's true life begins
- Warren entrances open fully
- Smuggling boats launch
- Death theaters perform
- Information changes hands

**Deep Night (12 AM):**
- Only the desperate or dangerous move
- Ranger night watch peaks
- Deep Warren activities hidden
- Emergency shelters on standby
- The island holds its breath

#### Social Customs & Culture

**Survival Etiquette:**
- "Play dead until ready" - strategic patience
- Never count Rangers before they return
- Touch wood before major decisions
- Sanctuary is absolute - violators die
- The ferry owes nothing to anyone

**Cultural Traditions:**

***Death Playing***: The opossum art of strategic withdrawal
- Formal version performed in theaters
- Practical version saves lives daily
- Children learn before walking
- Metaphor for island life
- "The best victory is survival"

***Ranger Nights***: Celebrating returning patrols
- Buying drinks for the living
- Toasting the unnamed fallen
- Trophy displays and story time
- Recruitment drives for replacements
- Dawn hangovers and regrets

***The Counting***: Annual memorial for all lost
- Names read from the Wall
- Families receive death tokens
- Moment of silence at noon
- Black market closes (only day)
- Even the Warrens observe

***Storm Solidarity***: When disaster threatens
- All feuds temporarily suspended
- Shelters open regardless of payment
- Resources shared for survival
- Rangers coordinate evacuation
- The island unites or dies

### The Rangers in Detail

#### Becoming a Ranger

**Why Creatures Join:**
- Desperation: No other options left
- Glory: Young creatures seeking fame
- Revenge: Lost family to titans
- Redemption: Criminals earning clean slate
- Madness: Some just want to fight giants

**Training Program:**

*Week 1-2: Basic Survival*
- Physical conditioning in full gear
- Titan biology and weak points
- Team coordination drills
- Emergency medical training
- Equipment familiarization

*Week 3-4: Advanced Combat*
- Live predator training (small ones)
- Trap construction and placement
- Poison and chemical weapons
- Coordinated attack patterns
- Survival psychology

*Week 5-6: Field Operations*
- Mainland patrol participation
- Titan tracking techniques
- Real encounter observation
- Final evaluation mission
- The Oath or the Exit

**The Ranger's Oath:**
"I stand between the city and the dark. I face what others flee. I guard those who cannot guard themselves. My life for the burrow. My death for the future. Until the titans fall or I fall, I am the wall."

#### Ranger Operations

**Patrol Types:**
- **Dawn Sweep**: Check overnight titan movement
- **Deep Range**: Multi-day penetration missions
- **Reaction Force**: Rapid response to sightings
- **Trap Maintenance**: Checking/resetting defenses
- **Recovery**: Retrieving fallen Rangers

**Combat Doctrines:**
- Never engage alone unless desperate
- Blind first, poison second, kill last
- Use terrain and creature advantages
- Acceptable losses calculated beforehand
- Recovery of wounded prioritized

**Equipment Loadouts:**

*Basic Ranger Kit:*
- Reinforced leather armor
- Species-specific weapons
- Three poison quills
- Two flash powder charges
- Emergency beacon
- First aid supplies
- One week rations

*Specialist Additions:*
- Scout: Far-sight scopes, wing reinforcement
- Trapper: Cable spools, anchor spikes
- Heavy: Improved armor, giant-killer weapons
- Medic: Extended supplies, stimulants
- Leader: Communication gear, maps

\columnbreak

#### Famous Rangers & Operations

**Legendary Figures:**

***Björn Bearsbane***: Only known solo bear kill
- Used avalanche trap in mountain pass
- Lost entire team before success
- Refused promotion, died on patrol
- Claw displayed in Trophy Hall
- Name inscribed in gold on Wall

***Silent Wing***: Bat scout extraordinaire
- Mapped giant hibernation sites
- Never lost on 200+ missions
- Trained three generations
- Vanished on final patrol
- Some say still out there

***The Mole Squad***: Underground specialists
- Developed pit trap techniques
- Saved 300 during moose rampage
- Lost half members to cave-in
- Survivors train new trappers
- Memorial tunnel named for them

**Historic Operations:**

***The Bark Flats Victory***: First coordinated bear kill
- Fifty Rangers deployed
- Twenty-seven casualties
- Three-day running battle
- Poison finally dropped beast
- Established modern tactics

***The Great Mauling***: Island's darkest day
- Bear reached Old Town
- Rangers fought street by street
- Hundred creatures lost
- Finally driven off at dawn
- Led to Heights fortification

***Operation Deep Strike***: Preemptive titan disruption
- Attacked deer during rut
- Scattered herds from city
- Twelve Rangers didn't return
- Bought six months peace
- Controversial but effective

### Crime & Shadow Operations

While Rangers represent the island's noble aspect, the shadow economy reveals its darker nature. Crime on Scurry Island isn't just tolerated—it's essential infrastructure.

#### Major Criminal Organizations

**The Fence Lords**: Controlling stolen goods flow
- Network spans all five burrows
- Sophisticated cleaning operations
- Protection for sellers and buyers
- Information as secondary commodity
- "Everything has a buyer somewhere"

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

**The Silent Tails**: Information brokerage supreme
- Ferret-dominated but species diverse
- Sell secrets to highest bidder
- Blackmail as business model
- Counter-intelligence services
- "We know what you did"

**The Deep Runners**: Warren control and smuggling
- Control underground route access
- Smuggling tunnels to mainland
- Hiding services for fugitives
- Fighting pit management
- "What happens below stays below"

#### Criminal Culture

**The Code of Shadows:**
1. Island business stays island business
2. No violence during sanctuary hours
3. Children and elders are off limits
4. Pay debts or pay consequences
5. Rangers get professional courtesy

**Status in the Underworld:**
- Reputation built on reliability
- Violence capability respected but not required
- Information is ultimate currency
- Connections matter more than species
- Survival trumps mainland morality

### Relationships with Other Burrows

#### Mousehattan - Necessary Evil
- **Economic**: Black market for rich mice's vices
- **Criminal**: Where problems get disappeared
- **Political**: Useful threat to keep others in line
- **Social**: "Those poor creatures on that awful island"
- **Reality**: More connected than anyone admits

**Typical Interactions:**
- Rich mice need discrete services
- Stolen goods flow both directions
- Information brokerage crucial
- Scapegoat for mainland problems
- Secret investments in island operations

#### The Branchx - Working Class Understanding
- **Economic**: Contraband construction supplies
- **Criminal**: Some failed workers flee here
- **Political**: Shared distrust of Mousehattan
- **Social**: "They're tough like us"
- **Reality**: More sympathy than expected

**Connections:**
- Union connections for smuggling
- Shared working-class values
- Some Rangers recruited from Branchx
- Construction expertise after storms
- "Better than the ground" mentality

#### The Hives - Cautious Commerce
- **Economic**: Agricultural goods and substances
- **Criminal**: Source for drug ingredients
- **Political**: Mutual outsider status
- **Social**: "Different but not enemies"
- **Reality**: Pragmatic relationship

**Trade Relations:**
- Exotic foods through black market
- Some beetles for fighting pits
- Information about other burrows
- Emergency food during shortages
- Careful distance maintained

#### Lin's Brook - Criminal Partnership
- **Economic**: Smuggling routes essential
- **Criminal**: Deep family connections
- **Political**: Allied against Mousehattan
- **Social**: "They understand survival"
- **Reality**: Closest mainland ally

**Joint Operations:**
- Underwater smuggling routes
- Shared criminal intelligence
- Some Rangers from Brook families
- Mutual protection agreements
- "Water connects us all"

### Notable NPCs

#### The Powers That Be

**Watch Commander Grimjaw**: One-eyed badger leading Rangers
- Lost eye to bear five years ago
- Promoted from ranks, not appointed
- Harsh but fair with recruits
- Drinks alone at Last Stop
- "Every Ranger is already dead"

**Mother Pale**: Ancient opossum matriarch
- Maintains sanctuary law through fear
- Knows everyone's secrets
- Never leaves Old Town
- Death playing master
- "I've outlived them all"

**Big Scar**: Raccoon crime lord
- Controls major smuggling routes
- Missing half his tail
- Reasonable unless crossed
- Protects his creatures
- "Business is just survival"

**The Ferryman**: Current boat controller (identity shifts)
- Whoever controls working ferry
- Position changes regularly
- Ultimate power over access
- Usually corrupt, always vital
- "The ferry sails when I say"

#### The Operators

**Lucky Silverpaw**: One-eyed raccoon gambling boss
- Runs the biggest fighting pit
- Never forgets a debt
- Fair odds, brutal collection
- Former Ranger himself
- "Luck is just good planning"

**Streak the Fence**: Ferret acquisition specialist
- Can find anything for anyone
- Loyalty bought not earned
- Network spans all burrows
- Prices always fair
- "Give me three days"

**Doc Patches**: Opossum running no-questions clinic
- Former mainland doctor
- Fled after "incident"
- Treats anyone who pays
- Drunk but competent
- "I don't remember faces"

**Silent Sara**: Scarred survivor turned trainer
- Three titan encounters lived
- Trains Ranger recruits
- Never speaks, only signs
- Toughest creature on island
- *Signs: "Words are for the living"*

\columnbreak

#### The Underground

**The Deepest**: Unknown Warren controller
- Identity complete mystery
- Controls deep tunnels
- Communicates through proxies
- Judge of Warren law
- "The deep provides"

**Tooth and Nail**: Mated ferret information brokers
- Know everyone's business
- Sell to highest bidder
- Protected by all sides
- Never leave the Warrens
- "Information wants to be sold"

**Bloody Bella**: Rabbit running fighting pits
- Escaped from Hives scandal
- Brutal but honest
- Maintains fighter medical
- Bets on every match
- "Blood makes the best ink"

### Adventure Hooks

#### Ranger Missions
- **Giant Migration**: Unusual deer movement threatens city - Rangers need intelligence
- **Missing Patrol**: Entire squad vanishes in Deep Woods - rescue or recovery?
- **New Threat**: Unknown predator species spotted - capture for study
- **The Blessed Quest**: Veteran Rangers seek titan young - insane or genius?
- **Poison Problems**: Supply of paralytic toxin runs low - dangerous harvest needed

#### Shadow Operations
- **War Brewing**: Fence Lords clash over territory - choose sides or stay neutral
- **Information Leak**: Someone's selling Ranger intelligence to unknown buyers
- **Deep Discovery**: Ancient ruins found in deepest Warrens - what did builders hide?
- **Sanctuary Violated**: Murder in neutral ground demands investigation
- **The Big Score**: Legendary theft needs crew - wealth or death awaits

#### Island Survival
- **Ferry Crisis**: All boats sabotaged simultaneously - island cut off completely
- **Storm of Century**: Hurricane approaches - evacuate or bunker down?
- **Plague Ship**: Sick refugees arrive - help them or protect island?
- **Titan Assault**: Coordinated predator attack - last stand time
- **The Counting Early**: Mass casualties demand answers - what's killing Rangers?

#### Political Intrigue
- **Independence Movement**: Island seeks formal separation - revolution brewing
- **Mainland Cleanup**: Mousehattan plans forced gentrification - resist or profit?
- **Ranger Coup**: Military considers taking full control - democracy or security?
- **Black Market War**: Competing syndicates escalate - innocents caught between
- **The Bridge Proposal**: Build permanent connection - salvation or destruction?

### GM Guidance

#### Running Scurry Island

**Tone Balance:**
- Grimy but not hopeless
- Dangerous but survivable
- Criminal but with honor
- Isolated but connected
- Tough but caring

**Key Themes:**
- Survival above all else
- Reputation matters more than law
- Everyone has a price
- The past doesn't matter
- Tomorrow isn't guaranteed

**Environmental Challenges:**
- Weather always threatens
- Ferries break constantly
- Resources run scarce
- Titans loom always
- Isolation weighs heavy

Remember: Scurry Island is where The Great Burrow's comfortable illusions die. Here, the reality of tiny creatures in a giant's world becomes undeniable. Yet it's also where heroism shines brightest—where forgotten creatures become Rangers, where survivors build community, where the last free corner of the world refuses to surrender.

<div class='note wide'>

#### <u>Ranger Mission Generator</u>

Roll 2d6 or choose:

**2-3:** Titan sighting reconnaissance - gather intel without engagement  
**4-5:** Rescue mission for lost creatures in titan territory  
**6-7:** Escort duty for important figures through dangerous zones  
**8-9:** Investigate strange titan behavior or new migration patterns  
**10-11:** Sabotage mission to redirect titan movement away from city  
**12:** Desperate last stand - titan heading directly for populated area  

Rangers use cunning over strength. Success means redirecting threats, not defeating them.

</div>

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


## Infrastructure & Technology

<div class='read'>

*"Next stop, Grand Central Burrow!" The mole conductor's voice carries over the rumble of the Underground train. You grip the root-fiber strap as the car sways through a particularly tight turn. Around you, the morning commute presses close—a beaver engineer studying blueprint scratches on bark, two mice debating interest rates, a drowsy opossum heading home from night shift. The train car smells of earth, sweat, and that particular Underground mixture of mushroom and metal. Through the carved windows, tunnel lights flash past in hypnotic rhythm. This is how The Great Burrow moves, deep beneath predator and titan alike.*

</div>

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

\columnbreak

### Transportation Methods
Beyond the Underground, creatures navigate via rope bridges (47 major crossings in The Branchx), ferry services (when operational), courier networks, and private options from otter swimming services to rare bat flights. Emergency bark slides provide rapid descent in the canopy, though climbing back up is always harder.

<div class='note'>

#### <u>Travel Time Guidelines</u>

Use these rough estimates for cross-burrow travel:
- **Underground Express**: 30-45 minutes between burrows
- **Surface Travel**: 2-3 hours (daylight only, weather permitting)
- **Courier Speed**: 1 hour for urgent messages
- **On foot**: Full day journey with predator risks

Always factor in delays: broken trains, predator sightings, weather, and classic NYC-style "track work."

</div>

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

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

<div class='note'>

#### <u>Union Politics in Play</u>

Unions aren't just background - they're active forces:
- **Strike actions** can shut down entire burrows
- **Union cards** open doors (or close them)
- **Scabs** face social ostracization or worse
- **Union bosses** wield political power rivaling crime families

Players with union connections get <span class='boost'>b</span> to Streetwise in working-class areas but upgrade difficulty when dealing with management.

</div>

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

<div class='note'>

#### <u>Political Faction Mechanics</u>

Track party reputation with each faction (-5 to +5):
- **-5 to -3**: Active opposition, may face harassment
- **-2 to +2**: Neutral, business as usual
- **+3 to +5**: Allied, gain faction benefits

Actions supporting one faction often oppose another. Let players feel the weight of political choices through NPC reactions and available opportunities.

</div>

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

<div class='note'>

#### <u>Using Recent History</u>

The Great Burrow's history provides ready-made NPC motivations:
- **Species War veterans** still hold grudges
- **Flood survivors** obsess over infrastructure
- **Trampling orphans** grew up tough on Scurry Island
- **Old money families** remember "better times"

Every major NPC should reference at least one historical event that shaped them.

</div>

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

<div class='note'>

#### <u>Seasonal Campaign Hooks</u>

**Spring:** Flood rescue missions, romance subplots, new construction conflicts

**Summer:** Water shortage negotiations, tourist-related crimes, heat-induced tensions

**Fall:** Harvest sabotage mysteries, storage facility heists, preparation panics

**Winter:** Food smuggling operations, warmth-based social dynamics, isolation stories

Use seasons to drive urgency and change available resources/obstacles.

</div>

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

<div class='read'>

*The back room of the Squeakeasy reeks of fermented berries and fear. Don Salvatore Longtail sits behind his oak-burl desk, one paw resting on a ledger, the other hidden beneath. His whiskers twitch once—the only sign he's heard your proposal. Behind him, two gray-coated rats crack their knuckles. "You come to my establishment," the Don says slowly, each word precise as a needle, "on the day of my daughter's tail-binding, and you ask me this favor? Tell me, friend—what makes you think the Longtail Family needs anything from you?" The silence that follows is heavy as winter snow.*

</div>

In the shadows between legitimate business and outright banditry lies The Great Burrow's complex criminal underworld. These organizations follow their own codes, respect their own territories, and handle their own justice.

## The Commission

An informal council where major family representatives meet quarterly to resolve disputes and coordinate operations. Meeting locations rotate between neutral territories:
- **Central Crossing** (The Branchx): Bridge intersection for safe meetings
- **The Sanctuary** (Scurry Island): Traditional neutral ground
- **Underground Stations**: Specific platforms with temporary truces

<div class='note'>

#### <u>Running Crime Family Politics</u>

The Commission provides natural story hooks:
- **Territory disputes** need neutral mediators (the PCs)
- **Family wars** threaten civilian areas
- **Commission meetings** are perfect heist/assassination targets
- **Power vacuums** create violent succession crises

Remember: organized crime provides actual services. When families fight, garbage piles up and predators aren't warned about.

</div>

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

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

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

<div class="footnote">THE GREAT BURROW<BR />
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

<div class='note'>

#### <u>Insect Technology Failures</u>

When <span class='symbols'>h</span> or <span class='symbols'>d</span> appear on insect-tech checks:
- **Beetles** get distracted by food
- **Ants** follow old pheromone trails
- **Spiders** abandon silk mid-spin
- **Crickets** chirp at wrong times
- **Butterflies** migrate unexpectedly

Make failures humorous but consequential!

</div>

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

\columnbreak

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


<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

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


## Tier 3 Talents

### Burrow Boss *(Passive)*
Leadership position in burrow hierarchy. Add <span class='boost'>b</span><span class='boost'>b</span> to Leadership checks. Can call upon significant resources and followers. Gain political influence but also enemies.

### Ranger Elite *(Passive)*
Veteran of multiple titan encounters. Add <span class='boost'>b</span><span class='boost'>b</span> to all combat checks against large creatures. Gain access to advanced Ranger equipment and tactics.

\columnbreak

### Underground Railroad *(Active)*
Can help creatures disappear from their old lives and start new ones. Once per session, can provide false identity, safe passage, or sanctuary for any creature.

### Titan Affinity *(Passive)*
*Prerequisite: Survived an encounter with a Titan, or DM approval*
One of the Titan-related skills becomes a career skill for you, based on the titan you have encountered.

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

## Tier 4 Talents

### Burrow Legend *(Passive)*
Your reputation precedes you throughout the city. Add <span class='boost'>b</span><span class='boost'>b</span> to all social checks within your home burrow. Once per session, may call upon your reputation to gain a significant favor or resource.

### Titan Whisperer *(Active)*
Your connection to the giants runs deeper than most. Once per session, may attempt to communicate with or influence a titan's behavior. This requires a Formidable (<span class='difficulty'>d</span><span class='difficulty'>d</span><span class='difficulty'>d</span><span class='difficulty'>d</span><span class='difficulty'>d</span>) Knowledge (Titans) check.

### Master of Networks *(Passive)*
Your web of contacts spans the entire city. Start each session with 3 "favor tokens" that can be spent to gain information, resources, or assistance from contacts throughout The Great Burrow.

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

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

Your hoarding instincts are legendary. Increase your Encumbrance Threshold by 3. Once per session, may produce a useful common item that you "had stored away" without use of a story point.

### Beaver Engineering *(Passive)*
*Prerequisite: Beaver species*

Your construction expertise is unmatched. When making Mechanics checks related to building or repair, add <span class='boost'>b</span><span class='boost'>b</span> to the check and reduce the time required by half.

### Otter Flow *(Passive)*
*Prerequisite: Otter species*

Your natural grace in water extends to all movement. Add <span class='boost'>b</span> to all Athletics and Coordination checks. When in water, upgrade the ability of these checks once.

### Rabbit Warren Leader *(Passive)*
*Prerequisite: Rabbit species*

Your community instincts make you a natural organizer. When leading a group of 3 or more creatures, all group members gain <span class='boost'>b</span> to checks that benefit from coordination. You may use Leadership instead of other social skills when dealing with family or community matters.

\columnbreak

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

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

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

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

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


<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

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

\columnbreak

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

\columnbreak

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

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

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

<div class='note'>

#### <u>Using Random Tables Wisely</u>

These tables are tools, not tyrants:
- **Foreshadow** results with warning signs
- **Adjust severity** based on story needs
- **Combine results** for complex situations
- **Let players influence** outcomes with preparation

Random doesn't mean arbitrary - make it feel inevitable in hindsight.

</div>

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

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

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

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

#### The Ranger Corps

**Scurry Island Rangers - Elite Military**
- **Allied (+3):** Full military support and resources, access to advanced weapons and training, protection during titan encounters, emergency evacuation assistance. Can request Ranger intervention in major threats.
- **Friendly (+2):** Basic military training opportunities, access to some Ranger equipment, assistance during emergencies, protection from external threats.
- **Neutral (0):** Standard interactions with military personnel and services.
- **Unfriendly (-2):** Exclusion from military assistance, difficulty accessing Ranger services, potential surveillance, reduced protection during emergencies.
- **Hostile (-3):** Active military opposition, denial of emergency services, potential arrest or detention, targeting as security threat.

\columnbreak 
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

\columnbreak 
<div class='example'>

##### Reputation in Action
Marcus the rat courier has been doing jobs for the Whisker Family, raising his reputation with them from Neutral to Friendly (+2). This gives him access to some illegal services and protection from petty crime.

However, his growing crime family connections have made him Unfriendly (-2) with the legitimate Branchx unions, who suspect he's working for the bosses who exploit workers.

</div>

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

## Arts and Entertainment

The Great Burrow's cultural life reflects diverse species and unique urban forest challenges.

### Theater and Performance

#### The Grand Oak Theater *(Mousehattan)*
- **Location:** Carved into the base of the Trading Oak
- **Capacity:** 800 creatures across four tiers
- **Programming:** Classical dramas, modern comedies, musical revues
- **Audience:** Primarily upper-class mice and rats
- **Notable Productions:** "The Merchant of Mousehattan," "A Midsummer Night's Squeak"

#### The People's Stage *(The Branchx)*
- **Location:** Natural amphitheater formed by intersecting branches
- **Capacity:** 1,200 creatures, standing room only
- **Programming:** Union rallies, folk performances, political satire
- **Audience:** Working-class creatures from all burrows
- **Notable Productions:** "The Nutcracker's Revenge," "Bridges of Madison County (Tree)"

#### The Crossroads Theater *(The Hives)*
- **Location:** Multiple venues throughout the burrow, rotating between districts
- **Programming:** Immigrant stories, fusion works, cultural celebrations
- **Audience:** Most diverse in the city, heavy working-class and immigrant attendance
- **Cultural Impact:** Showcases immigrant experiences and promotes cultural understanding

\columnbreak

### Visual Arts

#### The Mousehattan Museum of Natural Arts
- **Collection:** Ancient acorns, preserved leaves, mineral specimens, fossils
- **Special Exhibitions:** Rotating displays of contemporary creature art
- **Education Programs:** Art classes for young creatures
- **Controversy:** Debates over "modern" vs. "traditional" art

#### The Canopy Gallery Circuit *(The Branchx)*
- **Format:** Art displayed on bridge supports and tree trunks
- **Artists:** Working creatures creating in spare time
- **Themes:** Labor, community, resistance to gentrification
- **Medium:** Bark carvings, rope sculptures, found object installations

#### The Hives Cultural Collective
- **Focus:** Multicultural art celebrating immigrant traditions and fusion
- **Products:** Prairie dog pottery, marmot stonework, guinea pig textiles
- **Philosophy:** Art as bridge between cultures, celebrating diversity
- **Innovation:** Cross-cultural artistic techniques creating new art forms

<div class='note'>

##### <u>Cultural Venues by Burrow</u>

**Mousehattan:** Grand Oak Theater, Museum of Natural Arts, exclusive private galleries

**The Branchx:** People's Stage, Canopy Gallery Circuit, union-sponsored murals

**The Hives:** Crossroads Theater, Cultural Collective, rotating cultural festivals

**Lin's Brook:** Waterfront performance spaces, folk music traditions, craftsman workshops

**Scurry Island:** Death Theater, underground galleries, survival-themed performances

</div>

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

## Festivals and Celebrations

### The Great Burrow Calendar
**Seasonal Structure:** Spring Awakening (renewal, planting), Summer Growth (peak activity, construction), Autumn Harvest (gathering, gratitude), Winter Rest (reflection, community bonding)

### Major Festivals

#### The Great Awakening *(Spring Equinox)*
City-wide celebration of renewal and new beginnings. Communities plant new gardens, begin construction projects, and hold renewal ceremonies.

#### Midsummer Construction Festival
Celebrating the peak building season. Competitions between construction crews, displays of craftsmanship, and community barn-raising events.

\columnbreak

#### Harvest Gratitude *(Autumn Equinox)*
Thanksgiving for the year's abundance. Each burrow contributes traditional foods, cultural performances showcase diversity, and communities share resources for winter preparation.

#### The Long Night *(Winter Solstice)*
Community bonding during the darkest time. Underground gatherings with storytelling, planning for next year, and mutual aid distribution.


<div class="footnote">THE GREAT BURROW<BR />
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

<div class="footnote">THE GREAT BURROW<BR />
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

# Crime and Order

## The Rat Syndicate *(Primary Organized Crime)*
- **The Longtail Family:** Controls waterfront smuggling
- **The Whisker Brotherhood:** Runs protection rackets
- **The Gray Coats:** Newest family, challenging old territories

\columnbreak

## Crime Culture
- **"The Family Provides":** Code ensuring protection for those who pay
- **Tail Cutting:** Ultimate punishment for betrayal
- **The Bite:** Protection money paid monthly
- **Tunnel Wars:** Territorial disputes resolved underground

## The Underground Economy
- "Insurance" payments are a way of life
- Gambling and illegal seed trade
- Information brokerage through weasel networks
- Black market goods moving through hidden channels

# Daily Life

## Work Culture
- Dawn to past dusk standard for financial sector
- The Acorn Bell signals market open and close
- Whisker Break: Traditional mid-morning grooming/networking
- Complex social hierarchies based on address level

<div class='note'>

#### <u>Work as Story Driver</u>

Jobs aren't just background:
- **Workplace rivalries** create personal stakes
- **Professional skills** solve unexpected problems
- **Industry knowledge** reveals hidden connections
- **Economic pressure** forces moral compromises

Give each PC's profession at least one spotlight moment per session.

</div>

## Dealing with Giants
- Monthly evacuation drills for titan encounters
- The Hush: Children trained to freeze when warning bells ring
- Offering stations maintained to divert giant attention
- "Giant Insurance" is major business, often crime-family run

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

# Adventure Themes and Hooks

<div class='note'>

#### <u>Matching Themes to Players</u>

Different groups want different experiences:
- **Social players**: Political intrigue, crime family drama
- **Action players**: Predator encounters, gang warfare
- **Problem solvers**: Environmental crises, infrastructure disasters
- **Explorers**: External relations, lost districts

Start with one theme and weave in others as the campaign develops.

</div>

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
- **Leadership:** Don Salvatore Longtail
- **Specialties:** Protection rackets, loan sharking, tunnel smuggling
- **Code:** "The family provides" - honor-based obligations
- **Allies:** Traditional mouse families, conservative business interests
- **Enemies:** The Gray Coats, reform movements

### The Whisker Brotherhood *(New Money)*
- **Territory:** Financial district, new developments
- **Leadership:** Council of three brothers  
- **Specialties:** Business fraud, gambling, real estate schemes
- **Code:** "Make holes bigger" - expansion at any cost
- **Allies:** Rat entrepreneurs, corrupt officials
- **Enemies:** Longtail traditionalists, union organizers

### The Gray Coats *(Rising Power)*
- **Territory:** Times Squeak, entertainment districts
- **Leadership:** Lucia "The Shadow" Gray
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
