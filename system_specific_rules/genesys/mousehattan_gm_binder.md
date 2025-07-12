<style>
 .phb code {
     font-size:10px;
     padding-top: 0px;
     padding-bottom: 0px;
 }
/* IMPORTS */

@import url('https://fonts.googleapis.com/css?family=Crimson+Text:400,600,600i,700');

/* Main Background */
  .phb { background-image: url("https://i.imgur.com/5s6VJkT.png"); text-align:justify; text-indent:0px;}

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
    background-image: url('https://i.imgur.com/wk1XTwj.png');
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
    background-image: url('https://i.imgur.com/ks1JaPU.png');
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
    background-image: url('https://i.imgur.com/K1aEwZa.png');
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
    background-image: url('https://i.imgur.com/JEgri2b.png');
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

\pagebreakNum

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

## The Five Burrows

### Mousehattan - The Vertical Metropolis
The beating heart of commerce and ambition, carved into a rocky outcropping where ancient oak roots create natural highways. Wall Street is literally carved into walls, while Times Squeak never sleeps under managed firefly lighting.

### The Branchx - The Canopy Commons
Working-class pride sprawls through three dimensions high in ancient trees. Rope bridges span 47 major crossings, while emergency bark slides provide rapid descent - though climbing back up is always harder.

### The Hives - The Crossroads Community
The most diverse burrow, where prairie dogs organize democratic town halls next to traditional rabbit warrens, while mountain marmots work stone alongside guinea pig agricultural innovators.

### Lin's Brook - The Working Waterfront
Blue-collar pride on the waterfront where Whisker Creek meets tidal waters. The Great Dam powers workshops around the clock, while otter clans run ferry services and competitive slide-racing.

### Scurry Island - The Forgotten Burrow

Built on and around the massive fallen oak known as "The Old Giant," Scurry Island sits isolated in the central clearing where the forest opens to meadow. This is where creatures go to disappear, reinvent themselves, or make their fortune in the shadow economy. It's also home to the Rangers - those brave or foolish enough to venture beyond the city into the Deep Woods to face the titans.

#### The Fallen Giant
- **The Trunk:** Main thoroughfare, hollowed by generations into a covered market street
- **Root Town:** Maze-like neighborhood built in the exposed root system  
- **The Crown:** Dried branches form vertical neighborhoods, most dangerous
- **The Heartwood:** Deep interior chambers, some say it still lives

#### The Rangers
**Organization:** Watch Commander (grizzled badger), Scout Troops (flying squirrels and bats), Strike Teams (mixed species, heavily armed), The Blessed (survivors of direct titan encounters)

**Culture:** Recruitment from desperate creatures and glory seekers, six weeks training if you survive, "Between the city and the dark" oath

**Equipment:** Poison thorns, flash powder, trap lines, scent bombs, coordinated swarm attacks as last resort

#### Demographics & Economy
- **30% Opossums:** Masters of survival and adaptation
- **25% Raccoons:** Running most "businesses"
- **15% Rangers:** Mixed species, temporary residents
- **10% Fugitives:** From justice or debts elsewhere
- **20% Others:** The desperate, dreamers, and lost

**Black Market Central:** Contraband hub, fence operations, document forging, illegal substances, weapons trade

**The Titan Economy:** Bear season evacuations, trophy preparation, giant tracking information, evacuation services for the wealthy

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

<div class='example'>

##### Character Creation Example
Pip is creating a mouse character. She takes the mouse archetype (Brawn 1, Agility 2, Intellect 3, Cunning 2, Willpower 2, Presence 2) and decides to play an up-and-coming trader from Mousehattan. She chooses Charm and Negotiation as her starting skills and takes the Acorn Trader career for additional business skills.

</div>

<div class='note'>

#### <u>Additional Species</u>

The Core Rulebook includes 16 different species, including Opossums (The Survivors), Raccoons (The Operators), Otters (The Watercreatures), Badgers (The Old Guard), and many others. Each brings unique abilities and cultural perspectives to the Great Burrow.

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

<div class='note'>

#### <u>Career Paths and Advancement</u>

Characters can advance within their careers or cross-train into new ones as they gain experience. A Construction Worker might become a Union Organizer, or an Acorn Trader might develop connections to become a Crime Family Associate.

The key is that careers reflect not just skills, but social connections and cultural understanding within The Great Burrow's complex society.

</div>

<div class='example'>

##### Career in Action
Marcus the rat started as a Dock Worker in Lin's Brook but has been taking jobs from the Whisker Family crime organization. His player is spending XP to learn skills from the Crime Family Associate career, representing his growing involvement in organized crime.

Meanwhile, his childhood friend Bella the mouse parlayed her Construction Worker background into becoming a Union Organizer, using her understanding of working conditions to advocate for better treatment of laborers.

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

<div class='note'>

#### <u>Skill Applications in The Great Burrow</u>

Skills take on special meaning in the urban forest environment. Streetwise helps navigate the complex social networks of different burrows. Survival is useful not just in the wilderness, but in understanding the city's seasonal rhythms and resource cycles.

</div>

<div class="footnote">THE GREAT BURROW<BR />
<p>GENESYS RPG</p></div>

\pagebreakNum

# Arts and Entertainment

The Great Burrow's cultural life encompasses a rich tapestry of arts, entertainment, sports, and communication that reflects both the diverse species that call it home and the unique challenges of urban life in a forest world.

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

\\columnbreak

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

\\pagebreakNum

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

\\columnbreak

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

\\pagebreakNum

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

<div class='example'>

##### Using Species Manufacturing
A **Mouse-made Needle Sword** would have Damage 3, Crit 2, Range [Engaged], Encumbrance 1, Price 52 acorns (35 + 50%), *Pierce 1, Accurate 1*

A **Beaver-made Bark Plate** would have Soak +4 (+3 base +1 species), Defense 1, Encumbrance 5 (+1 species), Price 375 acorns (300 + 25%), *Cumbersome 1*

</div>

\columnbreak

## Weapons

### Traditional Weapons
- **Nutcracker Club:** Damage 4, Crit 4, Range [Engaged], Encumbrance 3, Price 20 acorns, *Knockdown*
- **Bark Bow:** Damage 5, Crit 3, Range [Long], Encumbrance 2, Price 40 acorns, *Prepare 1*
- **Needle Sword:** Damage 3, Crit 2, Range [Engaged], Encumbrance 1, Price 35 acorns, *Pierce 1*
- **Stone Axe:** Damage 5, Crit 3, Range [Engaged], Encumbrance 3, Price 25 acorns, *Vicious 1*

### Ranger Equipment
- **Poison Dart:** Damage 3, Crit 2, Range [Short], Encumbrance 0, Price 25 acorns, *Poison (stun)*
- **Entanglement Net:** Damage 1, Crit 6, Range [Short], Encumbrance 2, Price 50 acorns, *Ensnare 2*
- **Ranger Crossbow:** Damage 6, Crit 3, Range [Long], Encumbrance 3, Price 150 acorns, *Accurate 1, Prepare 1*

## Armor

### Light Armor
- **Work Clothes:** Soak +1, Defense 0, Encumbrance 1, Price 20 acorns
- **Leather Vest:** Soak +1, Defense 1, Encumbrance 1, Price 45 acorns
- **Courier Gear:** Soak +1, Defense 1, Encumbrance 1, Price 60 acorns, *Reduces falling damage by 1*

### Heavy Armor
- **Ranger Gear:** Soak +2, Defense 1, Encumbrance 3, Price 200 acorns, *Environmental protection*
- **Bark Plate:** Soak +3, Defense 1, Encumbrance 4, Price 300 acorns, *Cumbersome 1*
- **Shell Armor:** Soak +4, Defense 0, Encumbrance 5, Price 450 acorns, *Cumbersome 2, made from large insect shells*

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

## Transportation

### Personal Transport
- **Acorn Cap Boat:** Single creature, water travel, Price 100 acorns
- **Bark Sled:** Ground transport, can carry cargo, Price 50 acorns
- **Rope Harness:** For climbing/swinging, Price 25 acorns

### Public Transport
- **Underground Pass:** Monthly unlimited subway travel, Price 20 acorns
- **Ferry Ticket:** Single crossing to Scurry Island, Price 2 acorns
- **Courier Service:** Message delivery, Price 1-5 acorns depending on distance

\columnbreak

<div class='note'>

#### <u>Currency: The Acorn Standard</u>

The Great Burrow operates on the Acorn Standard, with currency valued by the quality and preparation of acorns:

- **Fresh Acorns:** Basic currency, 1-2 acorn value
- **Aged Acorns:** Higher value, 3-5 acorn value  
- **Prepared Acorns:** Processed and preserved, 5-10 acorn value
- **Prime Acorns:** Perfect specimens, 10+ acorn value

Trade also happens through barter, especially for specialized services and rare goods.

</div>

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

\columnbreak

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

<div class='note'>

#### <u>Titan-Touched Abilities</u>

Some talents reflect the mysterious phenomena that occasionally manifest in creatures who have survived direct encounters with the giants. These abilities are subtle and rare, often dismissed by urban dwellers as coincidence or delusion.

**Titan Affinity** allows characters to develop magical skills based on which titan they encountered, representing the deep psychological and spiritual impact of such experiences.

</div>

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

<div class='note'>

#### <u>Faction Benefits and Consequences</u>

**Allied (+3) with Mousehattan:** Access to exclusive financial services, business loans at favorable rates, invitations to high-society events, protection from economic retaliation.

**Hostile (-3) to The Branchx:** Blacklisting from union jobs, active sabotage of work projects, physical intimidation, exclusion from working-class communities.

**Friendly (+2) with The Hives:** Preferred access to honey and agricultural products, invitations to community gatherings, assistance with family matters.

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

\\columnbreak

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

\\pagebreakNum

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

\\columnbreak

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

\\pagebreakNum

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

\\columnbreak

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

\\pagebreakNum

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

\\columnbreak

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

\\pagebreakNum

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

\\columnbreak

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

\\pagebreakNum

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

\\columnbreak

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

\\pagebreakNum

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

\\columnbreak

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

\\pagebreakNum

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

\\columnbreak

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

\\pagebreakNum

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
| Season | Environmental | Social | Economic |
|:---:|:---:|:---:|:---:|
| **Spring** | Flooding, construction season | Mating season tensions | Building boom, trade revival |
| **Summer** | Heat, drought, peak titans | Tourism, social events | Peak trading, water costs |
| **Autumn** | Storms, preparation pressure | Harvest celebrations | Economic boom, hoarding |
| **Winter** | Cold, limited travel | Family gatherings, strain | Food scarcity, high costs |

##### Titan Encounter Responses
| Titan Type | Warning Time | Evacuation Scale | Duration |
|:---:|:---:|:---:|:---:|
| **Bear** | 30 minutes | City-wide | 2-6 hours |
| **Deer** | 60 minutes | Affected districts | 1-3 hours |
| **Moose** | 2+ hours | Regional | 4-12 hours |
| **Wild Boar** | 15 minutes | Local areas | 30 minutes-2 hours |

##### Crime Family Territory
| Family | Primary Burrow | Activities | Approach |
|:---:|:---:|:---:|:---:|
| **Longtail** | Mousehattan | Traditional protection | Honor, respect |
| **Whisker** | Mousehattan | Modern rackets | Business, profit |
| **Silverclaw** | Lin's Brook | Waterfront, smuggling | Practical, direct |
| **Shadow Runners** | Scurry Island | Black market, information | Survival, pragmatic |

</div>

##### Adventure Complications

| <span class='dice'>d</span><span class='dice'>d</span> | Complication |
|:---:|:---|
| 2-3 | Titan spotted approaching the area |
| 4-5 | Predator attack disrupts plans |
| 6-7 | Weather turns dangerous |
| 8-9 | Crime family gets involved |
| 10-11 | Union strike affects transportation |
| 12 | Government investigation launched |

\columnbreak

##### Random Encounters

| <span class='dice'>d</span><span class='dice'>d</span> | Underground | Surface | Canopy |
|:---:|:---|:---|:---|
| 2-3 | Tunnel flooding | Hawk patrol | Bridge maintenance |
| 4-5 | Train breakdown | Giant footprint | Nest robbers |
| 6-7 | Lost tourist | Market crowd | Rope bridge traffic |
| 8-9 | Crime family meeting | Street performance | Squirrel territory dispute |
| 10-11 | Mole strike | Courier race | Construction accident |
| 12 | Emergency evacuation | Titan offering ceremony | Crow gang recruitment |

<div class='read'>

*"The Great Burrow never sleeps. From the pre-dawn preparation of seed vendors to the after-midnight meetings in hidden speakeasies, this city pulses with the energy of creatures who refuse to be small. Every tunnel tells a story, every bridge represents a dream made real, and every citizen embodies the audacious spirit that built civilization in the shadow of giants."*

 From "A Newcomer's Guide to The Great Burrow" by Scholar Brightwhisker

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
<style>
    #p16{ display: none;}
</style>