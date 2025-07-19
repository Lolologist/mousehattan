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
    content: "•"; 
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

</style>


# The Smuggler's Cache
*A One-Shot Adventure for The Great Burrow*

In the gentrifying waterfront district of Lin's Brook, a hidden cache of valuable contraband has drawn the attention of multiple parties. What starts as a simple treasure hunt becomes a complex web of competing interests, moral choices, and the gray areas between legal and illegal that define life in the forest metropolis.

     This adventure tests characters' ability to navigate urban politics, species relationships, and the delicate balance between community and profit that shapes daily life in The Great Burrow. Success isn't just about claiming treasure - it's about understanding the consequences of choices in a city where everyone's connected to someone.

# Adventure Overview

## Setup Information

**Duration:** 3-4 hours  
**Players:** 4-6 characters  
**Tone:** Urban exploration with social intrigue and action  
**Themes:** Competing interests, moral choices, urban survival, species cooperation

### The Central Hook

While exploring an abandoned warehouse in the Greenbank district of Lin's Brook, the characters discover a hidden cache of valuable contraband. However, they're not the only ones looking for it - crime family enforcers from Mousehattan and desperate local smugglers are also converging on the location, all while trying to avoid the attention of burrow guards who would arrest everyone involved.

### The Stakes

- **Personal:** The cache contains 3,000 acorns worth of goods - enough to solve immediate financial problems and transform lives
- **Social:** Getting caught could ruin reputations and relationships across all five burrows
- **Political:** The contraband reveals corruption in the ferry system and trade regulations
- **Community:** How the situation resolves affects ongoing gentrification and working-class displacement in Lin's Brook

### Adventure Structure

The adventure unfolds through six key scenes, each building tension while offering multiple resolution paths:

1. **The Discovery** - Characters find the cache location
2. **The Watchers** - Local resident involvement and information gathering
3. **The Competition Arrives** - Three-way confrontation with competing parties
3.5. **The Silverclaw Intervention** - Guaranteed combat with territorial crime family
4. **The Law Arrives** - Authority involvement based on previous choices
5. **The Resolution** - Consequences and follow-up opportunities

<div class='note'>

#### <u>Running This Adventure</u>

**Flexible Beginning:** Characters can discover the cache through multiple means - accidental exploration, hired investigation, tip from informants, or following suspicious activity.

**Multiple Solutions:** Every scene has several resolution paths. Encourage creative problem-solving and negotiation over combat.

**Consequences Matter:** Choices affect reputation with different factions and create opportunities for future adventures.

**Urban Focus:** This is a city adventure - emphasize the interconnected nature of the community and how actions ripple outward.

</div>

<div class="footnote">THE SMUGGLER'S CACHE<BR />
<p>THE GREAT BURROW</p></div>

\pagebreakNum

## Background Information

### The Smuggling Operation

Three months ago, **Finn "Ripple" Shellcracker** (otter ferry operator) was running a small smuggling operation, moving luxury goods from Mousehattan to Scurry Island without paying proper tariffs. His contact was **Whiskers McGillicuddy** (mouse "import/export specialist") who had connections with the Longtail crime family of Mousehattan.

When a burrow guard investigation got too close, Finn panicked and hid his most valuable shipment in an abandoned warehouse, planning to retrieve it once things cooled down.

### The Complication

Finn was arrested two weeks ago on unrelated charges (drunk and disorderly during an otter slide race). In jail, he let slip details about the cache to his cellmate **Rusty Crowbar** (rat small-time criminal). Rusty has since been released and is planning to steal the cache.

Meanwhile, Whiskers has been pressuring the Longtail family to find the missing goods, leading to **Salvatore "Sal" Longtail** (rat crime family enforcer) being assigned to recover the shipment.

## Party Integration Hooks

*Specific roleplay opportunities based on your six-player party composition*

### Burl the Beaver (Dockworker)
**Reputation:** +2 Lin's Brook, +1 The Hives, -2 Longtail Family

**Built-in Connections:**
- **The Warehouse:** Burl worked on the original construction crew - he knows about the structural damage and secret spaces
- **Granny Driftwood:** She remembers him as "young Burl" and trusts him completely
- **Officer Tidecaller:** Professional respect as fellow working-class Lin's Brook resident
- **Longtail Conflict:** Sal recognizes him as "that beaver who cost us the dock contract" - instant tension

**Roleplay Hooks:**
- Burl can identify safe vs. dangerous areas of the warehouse
- Community members approach him for "the real story" about what's happening
- His dock union connections could provide backup or complications

### Cooper the Guinea Pig (Insect Wrangler)
**Reputation:** +2 The Hives, +1 Lin's Brook, -2 Mousehattan

**Built-in Connections:**
- **Silk Scarves in Cache:** Cooper recognizes these as Hives-made luxury goods, potentially his own work
- **Working Class Solidarity:** Immediate bond with other Lin's Brook working creatures
- **Mousehattan Distrust:** Upper-class NPCs dismiss him as "immigrant labor"

**Roleplay Hooks:**
- Can identify true value and origin of Hives goods in cache
- Guinea pig speech patterns (musical, code-switching) create cultural bridge-building opportunities
- Knowledge of terracing techniques might reveal hidden spaces in warehouse

### Lucius the Fox (Shadow Runner Associate)
**Reputation:** +2 Shadow Runners, +1 Lin's Brook, -2 Whisker Family

**Built-in Connections:**
- **Information Network:** Knows about the cache through Shadow Runner intelligence
- **Sal's Respect:** Crime family recognizes Shadow Runner neutrality
- **Whisker Family Tension:** They see him as "information leak" threat

**Roleplay Hooks:**
- Can provide background on all criminal players involved
- Shadow Runner code forbids direct confrontation but allows "finding lost items"
- Torn between Shadow Runner neutrality and personal gain

<div class="footnote">THE SMUGGLER'S CACHE<BR />
<p>THE GREAT BURROW</p></div>

\pagebreakNum

### Pine Bullseye (Chipmunk Ranger) 
**Reputation:** +2 Rangers, +1 Scurry Island, -2 Silverclaw Family

**Built-in Connections:**
- **Silverclaw Enemy:** Ripsaw attacks him on sight - guaranteed combat trigger
- **Law Enforcement Respect:** Officer Tidecaller knows Rangers help community
- **Underground Knowledge:** Ranger training reveals storm drain escape routes

**Roleplay Hooks:**
- Only character who can identify the Silverclaw threat early
- Chipmunk speed and ranger skills make him ideal scout and messenger
- Moral conflict between ranger duty and personal gain

### Willow the Private Investigator
**Reputation:** +2 Shadow Runners, +1 Whisker Family, -2 Longtail Family

**Built-in Connections:**
- **Professional Investigation:** Has legitimate reason to be investigating smuggling
- **Crime Family Tensions:** Caught between Shadow Runner neutrality and Whisker Family connections
- **Sal's Hostility:** Longtails see her as "that PI who asks too many questions"

**Roleplay Hooks:**
- Can legally question witnesses and examine evidence
- Professional ethics vs. criminal opportunity creates moral tension
- Whisker Family connection might provide inside information on Longtail operations

### Remy the Rat (Wannabe Chef)
**Reputation:** +2 Whisker Family, +1 Mousehattan, -2 Longtail Family

**Built-in Connections:**
- **Whisker Family Member:** Inside knowledge of family operations and rivalries
- **Mousehattan Foodie Scene:** Knows high-end restaurants and suppliers
- **Longtail Enemy:** Personal or family history creates immediate hostility with Sal's crew
- **Quality Ingredients:** Recognizes luxury food items in cache (honey liqueur, rare spices)

**Roleplay Hooks:**
- Can identify true value and authenticity of gourmet goods in cache
- Whisker Family loyalty vs. personal culinary ambitions creates internal conflict
- Rat speech patterns with food metaphors and culinary terminology
- Dreams of opening restaurant with cache money - legitimate business vs. crime family ties

## Pre-Adventure Character Backgrounds

*What each character has been doing leading up to the warehouse discovery*

### Burl the Beaver - Starting Character #1
**Recent Activity:** Working overtime shifts to pay for his elderly mother's medical care. His union boss mentioned "strange activity" around the old lumber warehouse where he used to work, and asked him to check it out unofficially.

**Integration Hook:** Burl approaches the warehouse alone initially, using his construction knowledge to scout the building. This gives him time to discover the structural issues and initial evidence before others arrive.

### Cooper the Guinea Pig - Starting Character #2  
**Recent Activity:** Investigating reports of stolen Hives silk being sold in Lin's Brook's black market. His legitimate work tracking insect-produced goods led him to suspicious warehouse activity.

**Integration Hook:** Cooper arrives shortly after Burl, recognizing the beaver from positive community reputation. Their shared working-class values create immediate common ground.

### Lucius the Fox - Character #3 (Second Wave)
**Recent Activity:** Received a Shadow Runner assignment to "observe and report" on unusual criminal activity in Lin's Brook. Not supposed to interfere, just gather intelligence.

**Integration Hook:** Lucius has been watching from a distance and approaches when he realizes Burl and Cooper might uncover something valuable. His Shadow Runner intel provides crucial background about all the criminal players involved.
<div class="footnote">THE SMUGGLER'S CACHE<BR />
<p>THE GREAT BURROW</p></div>

\pagebreakNum


### Pine Bullseye - Character #4 (Second Wave)
**Recent Activity:** Tracking Silverclaw smuggling operations through storm drains and underground routes. His ranger patrol brought him to investigate "structural instability" reports at the warehouse.

**Integration Hook:** Pine's ranger knowledge of underground routes gives the group alternative escape plans. His arrival also signals that dangerous forces (Silverclaws) will soon follow.

### Willow - Character #5 (Third Wave)
**Recent Activity:** Hired by a "concerned citizen" (actually Whiskers McGillicuddy) to investigate "suspicious insurance claims" related to the warehouse. She doesn't know her client's true criminal connections.

**Integration Hook:** Willow's legitimate investigation gives the group legal cover for being present. Her arrival coincides with discovering the actual cache, adding professional credibility to their claims.

### Remy the Rat - Character #6 (Final Addition)
**Recent Activity:** Sent by Whisker Family leadership to "check on their investment" after Whiskers McGillicuddy stopped reporting in. Told to assess the situation and report back, but his culinary ambitions make him see opportunity.

**Integration Hook:** Remy arrives during or just before the three-way confrontation, bringing crucial Whisker Family intel and immediate recognition of the cache's gourmet value. His presence forces final decisions about crime family loyalties vs. personal gain.

## GM Integration Strategies

### Recommended Staging

**Opening Scene (Burl + Cooper):**
- Start with these two discovering warehouse and initial cache evidence
- Establishes working-class cooperation and community stakes
- Gives time for initial exploration without overwhelming complexity

**Wave 2 (Add Lucius + Pine):**
- Lucius provides criminal intelligence, Pine adds ranger knowledge
- Creates tension: Shadow Runner neutrality vs. ranger law enforcement
- Introduces threat of Silverclaw retaliation through Pine's negative reputation

**Wave 3 (Add Willow + Remy):**
- Willow's investigation provides legal legitimacy
- Remy brings Whisker Family intel and gourmet goods expertise
- Group is now complete for complex multi-party negotiations with crime family insider knowledge

### Managing Group Dynamics

**Built-in Cooperation Incentives:**
- 3,000 acorn cache requires multiple characters to secure and transport
- Multiple crime family threats make allies essential
- Community connections (Lin's Brook +1 for three characters) encourage protecting neighborhood

\columnbreak

**Conflict Management:**
- Lucius vs. Willow professional rivalry creates roleplay tension without preventing cooperation
- Burl + Remy's Longtail hatred balanced by Pine's Silverclaw hatred - shared "enemy of my enemy" dynamic
- Cooper's outsider status makes him natural mediator between local factions
- Remy's Whisker Family loyalty vs. culinary dreams creates internal character tension that drives personal stakes

<div class='note'>

#### <u>Managing Party Tensions</u>

**Built-in Conflicts:**
- Lucius (Shadow Runner +2) vs. Willow (different Shadow Runner connection) - professional rivalry
- Burl (-2 Longtail) vs. Sal's crew - immediate hostility  
- Pine (-2 Silverclaw) vs. Ripsaw - combat inevitable
- Remy (-2 Longtail) vs. Sal's crew - family rivalry escalates tensions
- Remy (+2 Whisker) vs. Willow (+1 Whisker) - competing loyalty levels to same family

**Cooperation Incentives:**
- Multiple crime family threats make allies essential
- Community connections (Lin's Brook +1 for three characters) encourage protecting neighborhood
- Remy's Whisker Family intel + Willow's investigative skills = powerful information network

</div>

<div class="footnote">THE SMUGGLER'S CACHE<BR />
<p>THE GREAT BURROW</p></div>

\pagebreakNum

# Key NPCs

## Finn "Ripple" Shellcracker
*Otter Ferry Operator*

<div class="archetype">
<span class="bra">3</span>
<span class="agi">4</span>
<span class="int">2</span>
<span class="cun">2</span>
<span class="wil">1</span>
<span class="pre">3</span>
</div>

<div class="adversary">
<span class="soak">4</span>
<span class="wound">15</span>
<span class="strain">11</span>
<span class="mdef">1</span>
<span class="rdef">1</span>
</div>

**Skills:** Athletics 2 (**Water +2 <span class='boost'>b</span><span class='boost'>b</span>**), Coordination 2, Vehicles 2, Streetwise 1, Survival 1, Mechanics 1, Vigilance 1

**Talents:** 
- **Aquatic Excellence:** Add <span class='boost'>b</span><span class='boost'>b</span> to all swimming checks, hold breath for extended periods
- **Playful Competitor:** Add <span class='boost'>b</span> to Cool checks during stressful social situations
- **Water Sense:** Remove <span class='setback'>b</span> from Navigation checks near water
- **Slippery:** Add <span class='boost'>b</span> to escape restraints
- **Toughened:** Wound Threshold +2

**Equipment:** Reinforced vest, diving suit, rope, emergency rations, waterproof message tube

**Personality:** Nervous, talkative, tries to be helpful but makes things worse  
**Motivation:** Get out of jail and retrieve his cache without getting killed  
**Speech Pattern:** Fluid otter speech with dock worker slang and water metaphors  
**Current Status:** In Lin's Brook jail, available for questioning if characters visit

\columnbreak

<div class="read">

*A sleek brown otter sits hunched on the jail's stone bench, his usually glossy fur dulled and unkempt. His webbed paws fidget constantly, and his dark eyes dart nervously between you and the cell door. When he speaks, his voice carries the fluid cadence of his species but trembles with anxiety.*

"Oh, listen friends, I can explain everything - well, most of it flows together anyway. This whole mess swept me away like spring runoff, you know? One minute I'm sliding through a simple side business, next thing the current's got me tumbling tail over whiskers and I'm beached here while my whole life's work sits high and dry where even the king tide can't touch it. You seem like reasonable folk who know how to ride the current - maybe we can help each other navigate these rapids? No use swimming upstream alone, eh?"

</div>

**Key Information Finn Provides:**
- Exact location of the cache in the warehouse basement
- Combination to the lock (his daughter's birthday)
- Contents: honey liqueur, silk scarves, rare spices, luxury goods
- Warning about tidal timing - cache only accessible at low tide
- Mentions both Whiskers and "that crazy rat" (Rusty) as potential problems

<div class="footnote">THE SMUGGLER'S CACHE<BR />
<p>THE GREAT BURROW</p></div>

\pagebreakNum

## Whiskers McGillicuddy
*Mouse Import/Export Specialist*

<div class="archetype">
<span class="bra">1</span>
<span class="agi">2</span>
<span class="int">4</span>
<span class="cun">3</span>
<span class="wil">3</span>
<span class="pre">2</span>
</div>

<div class="adversary">
<span class="soak">2</span>
<span class="wound">9</span>
<span class="strain">16</span>
<span class="mdef">0</span>
<span class="rdef">0</span>
</div>

**Skills:** Mechanics 3 (**Tools +1 <span class='boost'>b</span>**), Knowledge (Science) 2, Perception 1, Vigilance 1, Coordination 1, Negotiation 2, Streetwise 2

**Talents:** 
- **Tunnel Sense:** Remove <span class='setback'>b</span> from Navigation checks in underground environments
- **Precise Work:** Add <span class='boost'>b</span> to all Mechanics checks
- **Social Networks:** Start with one contact in Mousehattan, and +1 reputation
- **Grit:** Strain Threshold +1

**Equipment:** Work clothes, tunnel digging kit, magnifying glass, firefly lantern, emergency rations

**Personality:** Smooth-talking, well-dressed, nervous about crime family pressure  
**Motivation:** Recover goods to satisfy Longtail family and save his reputation  
**Speech Pattern:** Precise mouse diction with business jargon  
**Location:** Mousehattan financial district, but will travel to meet characters

\columnbreak
<div class="read">

*An impeccably groomed mouse approaches, his gray fur perfectly combed and his tiny whiskers waxed to sharp points. He wears a miniature vest of fine cloth and carries himself with the practiced confidence of old Mousehattan money, though you notice his paws shake slightly as he adjusts his spectacles. His voice is cultured and precise, each word carefully chosen.*

"Good day. I am Whiskers McGillicuddy of McGillicuddy Import & Export, established 1887 - perhaps you've heard of our firm? Third generation in the trade, I'll have you know. I find myself in need of... discrete assistance regarding a matter of some considerable delicacy. Let us discuss this as civilized creatures, shall we? Time, as my grandfather always said, is more valuable than prime acorns, and I'm afraid my reserves of both are approaching critical depletion. Now then, to business - I trust we can conduct ourselves with appropriate decorum?"

</div>

<div class="footnote">THE SMUGGLER'S CACHE<BR />
<p>THE GREAT BURROW</p></div>

\pagebreakNum

## Salvatore "Sal" Longtail
*Rat Crime Family Enforcer*

<div class="archetype">
<span class="bra">2</span>
<span class="agi">2</span>
<span class="int">2</span>
<span class="cun">4</span>
<span class="wil">2</span>
<span class="pre">2</span>
</div>

<div class="adversary">
<span class="soak">3</span>
<span class="wound">13</span>
<span class="strain">13</span>
<span class="mdef">0</span>
<span class="rdef">0</span>
</div>

**Skills:** Streetwise 2, Stealth 2, Skulduggery 2, Deception 1, Vigilance 1, Coercion 2, Brawl 2, Ranged (Light) 1

**Talents:** 
- **Adaptable:** Once per session, may add <span class='boost'>b</span> to any skill check
- **Network Builder:** Reduce difficulty of Streetwise checks by 1 (minimum <span class='ability'>d</span>)
- **Survivor's Instinct:** Add <span class='boost'>b</span> to Vigilance and Cool checks
- **Nobody's Fool:** Upgrade difficulty of social checks targeting him
- **Sixth Sense:** Once per session add <span class='boost'>b</span><span class='boost'>b</span> to Vigilance/Perception

**Equipment:** Padded jacket, concealed knife, family identification, emergency funds

**Personality:** Professional, intimidating, surprisingly reasonable if treated with respect  
**Motivation:** Recover family property, maintain reputation, avoid unnecessary violence  
**Speech Pattern:** Confident rat speech with family metaphors  
**Resources:** 3-4 rat associates, crime family backing, knowledge of underground

\columnbreak

<div class="read">

*A large, well-built rat emerges from the shadows, his dark fur immaculately groomed and his posture radiating quiet authority. Unlike the flashy new-money rats of Mousehattan, he dresses simply but expensively - quality speaks louder than ostentation. His tail, longer than most, moves with deliberate control, and his dark eyes assess you with professional interest rather than hostility.*

"Hey there, good evening! Name's Salvatore Longtail - but please, call me Sal! I represent certain... family interests in this whole situation, yeah? Look, I understand there's some confusion about who owns what here - happens all the time in business, am I right? Nothing personal, you understand - we're just trying to make sure everyone gets their fair share of the pie. Maybe we can work something out that makes everybody happy? The family always appreciates when smart creatures cooperate - we got long memories for our friends, and we like to see everybody's hole get bigger, you know what I'm saying?"

</div>

<div class="footnote">THE SMUGGLER'S CACHE<BR />
<p>THE GREAT BURROW</p></div>

\pagebreakNum

## Rusty Crowbar
*Rat Small-time Criminal*

<div class="archetype">
<span class="bra">2</span>
<span class="agi">2</span>
<span class="int">1</span>
<span class="cun">3</span>
<span class="wil">1</span>
<span class="pre">1</span>
</div>

<div class="adversary">
<span class="soak">3</span>
<span class="wound">11</span>
<span class="strain">10</span>
<span class="mdef">0</span>
<span class="rdef">0</span>
</div>

**Skills:** Streetwise 2, Skulduggery 2, Stealth 1, Brawl 2, Survival 1, Vigilance 1

**Talents:** 
- **Street Rat:** Basic criminal abilities, familiar with urban survival
- **Desperate Fighter:** When wounded, add <span class='boost'>b</span> to Brawl checks

**Equipment:** Makeshift crowbar weapon (Damage 3, Crit 4), ragged clothes, stolen goods

**Personality:** Desperate, paranoid, quick to violence when cornered  
**Motivation:** Score big to pay off debts and get out of the city  
**Speech Pattern:** Street rat slang, nervous energy  
**Resources:** Improvised weapons, knowledge of abandoned buildings, nothing to lose

<div class="read">

*A scrawny rat with patchy fur and wild eyes skulks into view, clutching a makeshift weapon - a sharpened piece of metal that might once have been a crowbar. His clothes are mismatched and dirty, and he moves with the twitchy energy of someone who's been looking over his shoulder for too long. Scars crisscross his arms and face, telling stories of a hard life in the city's underbelly.*

"Well, well, well! Look what crawled outta the walls! More treasure hunters trying to muscle in on MY score, eh? Listen up, and listen good - I been working this angle for weeks, see? This cache is my ticket to swimming instead of sinking, and I ain't letting nobody - NOBODY - take food outta my mouth! You seem like smart folk who know which way the current flows - so turn around and scurry back where you came from before somebody gets hurt. This is my ONE SHOT to stop scraping barnacles off the bottom, and I'll bite through anyone who tries to stop me!"

</div>

<div class="footnote">THE SMUGGLER'S CACHE<BR />
<p>THE GREAT BURROW</p></div>

\pagebreakNum

\pagebreakNum

## Officer Marina Tidecaller
*Otter Burrow Guard*

<div class="archetype">
<span class="bra">2</span>
<span class="agi">3</span>
<span class="int">2</span>
<span class="cun">2</span>
<span class="wil">3</span>
<span class="pre">2</span>
</div>

<div class="adversary">
<span class="soak">4</span>
<span class="wound">12</span>
<span class="strain">14</span>
<span class="mdef">1</span>
<span class="rdef">1</span>
</div>

**Skills:** Athletics 2 (**Water +2 <span class='boost'>b</span><span class='boost'>b</span>**), Vigilance 2, Perception 2, Coercion 1, Leadership 1, Knowledge (City) 2, Brawl 1, Ranged (Light) 1

**Talents:** 
- **Aquatic Excellence:** Add <span class='boost'>b</span><span class='boost'>b</span> to all swimming checks, hold breath for extended periods
- **Playful Competitor:** Add <span class='boost'>b</span> to Cool checks during stressful social situations
- **Natural Leader:** Add <span class='boost'>b</span> to Leadership checks when coordinating water-based activities
- **Law Enforcement Training:** May use Authority instead of Coercion in official capacity

**Equipment:** Guard uniform with badge, official weapon, restraints, communication device

**Personality:** Dedicated, fair but strict, knows the neighborhood well  
**Motivation:** Keep the peace, investigate suspicious activity, protect community  
**Speech Pattern:** Authoritative otter speech with water metaphors  
**Resources:** Legal authority, backup guards, knowledge of local crime

\columnbreak

<div class="read">

*A sturdy otter in the blue-gray uniform of the Lin's Brook Guard approaches with confident, measured steps. Her badge gleams against her dark brown fur, and her keen eyes miss nothing as they sweep the area. She carries herself with the easy authority of someone who knows her beat intimately and takes pride in protecting it.*

"Well now, what's all this splashing about, citizens? I've had reports of suspicious activity in this area, and I can see the current's running strange today. This warehouse has been dry-docked for months, and suddenly there's more traffic than spawning season at the falls. I know most of you by sight - you swim in my waters regular-like - but some faces are new to this stretch of the creek. Mind explaining what brings you all to this particular eddy on my beat? And let's keep it smooth as a morning swim, shall we?"

</div>

<div class="footnote">THE SMUGGLER'S CACHE<BR />
<p>THE GREAT BURROW</p></div>

\pagebreakNum

## Granny Driftwood
*Beaver Local Resident*

<div class="archetype">
<span class="bra">3</span>
<span class="agi">1</span>
<span class="int">2</span>
<span class="cun">3</span>
<span class="wil">3</span>
<span class="pre">2</span>
</div>

<div class="adversary">
<span class="soak">4</span>
<span class="wound">14</span>
<span class="strain">14</span>
<span class="mdef">0</span>
<span class="rdef">0</span>
</div>

**Skills:** Perception 3, Vigilance 2, Knowledge (City) 3, Survival 2, Mechanics 2, Leadership 1

**Talents:** 
- **Master Builder:** Add <span class='boost'>b</span> to all Mechanics checks involving construction
- **Aquatic:** Can hold breath for extended periods, swim at full speed
- **Sturdy:** Increase soak value by 1
- **Neighborhood Watch:** Add <span class='boost'>b</span><span class='boost'>b</span> to Perception checks when observing familiar areas

**Equipment:** Comfortable home furnishings, binoculars, tea service, emergency supplies

**Personality:** Elderly, observant, protective of neighborhood, suspicious of outsiders  
**Motivation:** Preserve community character, watch out for trouble  
**Speech Pattern:** Deliberate beaver speech with construction metaphors  
**Location:** Lives across from warehouse, watches everything from her window

\columnbreak

<div class="read">

*An elderly beaver sits in her window, a steaming cup of bark tea in her weathered paws and a pair of well-used binoculars around her neck. Her gray-streaked fur is neatly groomed, and she wears a hand-knitted shawl that speaks of practical comfort over fashion. Her lodge is clearly well-maintained - a testament to beaver craftsmanship and pride.*

"Well now, what's all this construction without permits? More strangers poking around that old warehouse, I see. In my day, creatures understood that good fences make good neighbors, and you didn't go gnawing on timber that wasn't yours. That building's foundation has been rotting since the lumber company moved out - weak supports bringing all sorts of unsavory types to undermine our neighborhood's structural integrity. You seem different from the others, though. Got the look of creatures who know quality work when they see it. Care to tell an old beaver what kind of demolition or renovation is really going on over there? Because from where I sit, that whole structure looks ready to collapse."

</div>

<div class="footnote">THE SMUGGLER'S CACHE<BR />
<p>THE GREAT BURROW</p></div>

\pagebreakNum

## Supporting NPCs

### Sal's Associates (3-4)
*Rat Crime Family Muscle*

**Characteristics:** Brawn 2, Agility 2, Intellect 1, Cunning 2, Willpower 2, Presence 1

<div class="minion">
<span class="soak">3</span>
<span class="wound">3</span>
<span class="mdef">0</span>
<span class="rdef">0</span>
</div>

**Skills (Group Only):** Brawl 2, Ranged (Light) 1, Streetwise 1, Skulduggery 1

**Talents:** 
- **Species Variant - Rats:** Add <span class='boost'>b</span> to Streetwise checks in urban environments
- **Family Loyalty:** Add <span class='boost'>b</span> to checks when supporting Sal

**Equipment:** Concealed weapons (knives/clubs, Damage 3, Crit 4), nice clothes, family identification

### Rusty's Desperate Allies (1-2)
*Street Scavengers*

**Characteristics:** Brawn 2, Agility 2, Intellect 1, Cunning 2, Willpower 1, Presence 1

<div class="minion">
<span class="soak">2</span>
<span class="wound">3</span>
<span class="mdef">0</span>
<span class="rdef">0</span>
</div>

**Skills (Group Only):** Brawl 1, Skulduggery 2, Survival 1, Stealth 1

**Talents:** 
- **Species Variants:** 
  - **Mice:** Add <span class='boost'>b</span> to Stealth checks when hiding
  - **Squirrels:** Add <span class='boost'>b</span> to Athletics checks for climbing
- **Desperate:** When wounded, add <span class='boost'>b</span> to Brawl checks

**Equipment:** Improvised weapons (Damage 2, Crit 5), scavenged clothing, stolen goods

<div class="footnote">THE SMUGGLER'S CACHE<BR />
<p>THE GREAT BURROW</p></div>

\pagebreakNum

# Key Locations

## The Abandoned Warehouse
*Primary Adventure Location*

### Overview
A three-story brick building on the Greenbank waterfront, formerly used for storing lumber. Now empty due to gentrification, with broken windows, a "For Lease" sign, and the general air of urban decay giving way to "development opportunity."

### Sensory Description

<div class="read">

*The warehouse greets you with the musty scent of old wood and damp stone, mixed with the salt tang of the nearby waterfront. Creaking timbers echo your footsteps as loose floorboards groan underfoot, while shafts of dusty sunlight filter through broken windows, casting dancing shadows across water-stained walls. The rhythmic lapping of waves against the dock below provides a constant backdrop, punctuated by the distant calls of dock workers and the occasional screech of rusty hinges. Your paws feel the gritty texture of sawdust and debris, while the air tastes of brine and decay - a monument to Lin's Brook's industrial past now surrendering to an uncertain future.*

</div>

### Layout

#### Ground Floor
- **Open Space:** Former lumber storage with old racks still visible
- **Loading Dock:** Large doors facing the waterfront, some still functional
- **Foreman's Office:** Small room with desk, paperwork, view of main floor
- **Challenges:** Loose floorboards, debris, multiple entrances

#### Second Floor
- **Storage Rooms:** Smaller chambers for specialized materials
- **Supervisor's Office:** Good view of street, overlooks Granny Driftwood's house
- **Challenges:** Weak stairs, holes in floor, but excellent observation points

\columnbreak

#### Basement *(Cache Location)*
- **The Hidden Cache:** Behind false wall, accessible only at low tide
- **Flooding:** Basement floods during high tide, making access dangerous
- **Contents:** 50 bottles honey liqueur, silk scarves, rare spices, luxury goods
- **Total Value:** 1,400 acorns
- **Challenges:** Tidal timing, structural damage, concealed entrance

<div class='note'>

#### <u>Warehouse Challenges</u>

**Timing with Tides:** Cache only accessible during low tide (6-hour cycles)
**Structural Damage:** Unsafe floors, loose boards, weak stairs
**Multiple Entrances:** Easy to be surprised by other parties
**Visibility from Street:** Granny Driftwood watches everything
**Sound Carries:** Noise alerts neighbors and other interested parties

</div>

### The Cache Contents

| Item | Quantity | Unit Value | Total Value |
|:---|:---:|:---:|:---:|
| Premium Honey Liqueur | 75 bottles | 12 acorns | 900 acorns |
| Silk Scarves (Hives) | 15 pieces | 25 acorns | 375 acorns |
| Rare Spices (Coastal) | 12 containers | 40 acorns | 480 acorns |
| Luxury Goods (Mousehattan) | 15 items | 50 acorns | 750 acorns |
| Imported Jewelry | 5 pieces | 100 acorns | 500 acorns |
| **Total Cache Value** | | | **3,000 acorns** |

For perspective: This represents enough wealth to buy a large family estate, 8-10 months wages for skilled workers, or could fund a substantial business venture. This is life-changing money that would attract serious attention from all major criminal organizations.

**Remy's Expertise:** As a wannabe chef with Whisker Family connections, Remy can immediately identify the premium quality of these goods. The honey liqueur is from exclusive Hives apiaries, the spices are coastal imports worth triple their weight, and the luxury goods include rare Mousehattan delicacies he's only dreamed of cooking with.

<div class="footnote">THE SMUGGLER'S CACHE<BR />
<p>THE GREAT BURROW</p></div>

\pagebreakNum

## Granny Driftwood's House
*Observation Post and Information Hub*

### Description
Well-maintained beaver lodge built into the waterfront embankment with a perfect view of the warehouse. Granny sits by her window with tea and binoculars, making her the neighborhood's unofficial security system.

### What Granny Has Observed
- **Rusty Crowbar:** Casing the building for several days, acting suspicious
- **Well-dressed Mouse:** Whiskers asking questions yesterday, very nervous
- **Rat Associates:** Several well-dressed rats in the area this morning
- **Ferry Schedules:** Knows the tidal timing and local routines

### Roleplay Opportunities
- Information gathering about recent activity
- Negotiating for her silence or cooperation  
- Learning neighborhood history and concerns
- Getting warnings about approaching trouble
- Understanding community impact of gentrification

## The Dockside Tavern
*Optional Information Hub*

### Description
Working-class otter bar where dock workers gather after shifts. Dim lighting, water-stained wood, competitive slide-racing stories, and the smell of fish and fermented beverages.

### Notable NPCs
- **Barkeep Splash** (otter): Knows everyone, trades information for drinks
- **Various Dock Workers:** Gossip about smuggling, crime families, recent arrests

### Information Available
- Finn's arrest and jailhouse gossip about hidden treasure
- Recent crime family activity in the area
- Smuggling routes and methods used by local operators
- Community concerns about gentrification and rising rents

## Lin's Brook Jail
*Optional Location for Finn Interview*

### Description
Small holding facility built into a converted beaver dam section. Secure but not maximum security, designed for local troublemakers rather than serious criminals.

### Visiting Requirements
- Convincing Officer Tidecaller with good reason
- Small bribe (5-10 acorns) to guard
- Official business (fake or real)
- Family connection claim

### Risks
- Finn is eager to talk but other prisoners might overhear
- Guards are suspicious of unusual visitors
- Information might reach wrong ears
- Future complications if discovered


<div class="footnote">THE SMUGGLER'S CACHE<BR />
<p>THE GREAT BURROW</p></div>

\pagebreakNum

## Greenbank Ferry Terminal
*Potential Escape Route*

### Description
Small dock with irregular ferry service to other parts of the city. Currently under renovation, creating both hiding spots and obstacles for characters trying to escape with goods.

### Tactical Considerations
- Multiple escape routes by water for those who can swim
- Construction equipment provides cover during confrontations
- Ferry schedules affect timing - may not be available when needed
- Officer Tidecaller patrols here regularly

<div class='note'>

#### <u>Using Locations Effectively</u>

**The Warehouse** serves as the central location but shouldn't confine the entire adventure. Let characters explore the neighborhood.

**Granny's House** provides crucial exposition and shows community impact. Her reaction to events affects the adventure's tone.

**Optional Locations** add depth and give characters choices about how to approach problems. Not every location needs to be visited.

**Environmental Storytelling** - Each location should reinforce themes of gentrification, community change, and the tension between old and new ways of life.

</div>

\columnbreak

### Location Quick Reference

| Location | Primary Use | Key NPCs | Information Available |
|:---|:---|:---|:---|
| **Warehouse** | Cache location, main scenes | None (various visitors) | Cache contents, structural hazards |
| **Granny's House** | Information gathering | Granny Driftwood | Recent activity, tidal timing, community concerns |
| **Dockside Tavern** | Background information | Barkeep Splash, workers | Criminal activity, neighborhood gossip |
| **Jail** | Finn interview | Finn Shellcracker, guards | Cache location, smuggling details |
| **Ferry Terminal** | Escape route | Officer Tidecaller (patrols) | Transportation options, law enforcement |

<div class='example'>

##### Bringing Locations to Life

**Environmental Details:** The constant sound of water against wood, salt air mixing with urban smells, the contrast between traditional beaver craftsmanship and modern decay.

**Cultural Touches:** Otter work songs from the docks, beaver construction terminology in conversations, the particular way water-workers move and speak.

**Economic Pressure:** "For Lease" signs, boarded windows next to expensive renovations, longtime residents watching their neighborhood change around them.

</div>

<div class="footnote">THE SMUGGLER'S CACHE<BR />
<p>THE GREAT BURROW</p></div>

\pagebreakNum

# Scene Breakdown

## Scene 1: The Discovery
*30 minutes - Exploration and Investigation*

### Setup
Characters enter the warehouse through their chosen method. The building shows signs of recent activity - disturbed dust, footprints, evidence that others have been searching.

### Objectives
- Explore the building and assess its condition
- Discover signs of recent activity from other parties
- Find the basement entrance and understand the tidal timing
- Locate the hidden cache (requires investigation or Finn's information)

### Key Events
- Characters notice the warehouse has been visited recently
- Discovery of structural damage and safety hazards
- Realization that basement floods with tides
- Finding evidence of the cache's existence

### Possible Complications
- **Granny Driftwood Spots Them:** She calls out from her window, demanding to know their business
- **Structural Hazards:** Loose floorboards, weak stairs that could cause injury or noise
- **Tide Timing:** Urgency if the tide is coming in soon
- **Signs of Others:** Evidence that multiple parties have been here recently

\columnbreak

### Resolution
Characters should end this scene with knowledge of the cache location and an understanding that they're not alone in their interest. The scene sets up the social dynamics that will drive the rest of the adventure.

<div class='example'>

##### Discovery in Action

"You notice fresh scratches around the basement door - someone's been working on the lock recently. The dust patterns on the stairs show at least three different sets of prints: large ones that might be rat, smaller precise ones that could be mouse, and your own. Through the broken windows, you can see an elderly beaver across the street watching your every move with obvious interest."

</div>

<div class="footnote">THE SMUGGLER'S CACHE<BR />
<p>THE GREAT BURROW</p></div>

\pagebreakNum

## Scene 2: The Watchers
*20 minutes - Social Encounter*

### Setup
Granny Driftwood has been observing the warehouse and knows something's happening. She's protective of her neighborhood but also curious about the sudden activity.

### Key Roleplay Opportunities
- Learn about recent suspicious activity
- Negotiate for information or silence
- Understand community concerns about gentrification
- Get warnings about approaching trouble
- Discuss the neighborhood's history and changes

### Possible Outcomes

**Ally (+2 Reputation with Lin's Brook Community):**
- Granny helps watch for trouble and provides local knowledge
- Warns about approaching problems
- Offers safe haven if things go wrong
- Provides community context for decisions

**Neutral (No reputation change):**
- She stays out of it but won't actively help or hinder
- Provides basic information if asked politely
- May report illegal activity to authorities

**Hostile (-1 Reputation with Lin's Brook Community):**
- Calls the guards if characters seem threatening
- Spreads word about "troublemakers" in the neighborhood
- Actively opposes character goals

### Information Revealed
- Rusty has been casing the building for days
- A well-dressed mouse (Whiskers) was asking questions yesterday
- Several rats in nice clothes were in the area this morning
- Ferry schedules, tide times, and local routines
- Neighborhood concerns about crime and gentrification

<div class="footnote">THE SMUGGLER'S CACHE<BR />
<p>THE GREAT BURROW</p></div>

\pagebreakNum

## Scene 3: The Competition Arrives
*45 minutes - Tense Negotiation with Combat Potential*

### Setup
Just as characters are accessing the cache (or planning to), both Rusty and Sal's crew arrive. This creates a three-way standoff with multiple possible resolutions.

### Participants
- **Characters:** Trying to claim or escape with the cache
- **Rusty Crowbar + 1-2 Desperate Allies:** Armed with improvised weapons, nothing left to lose
- **Sal + 3-4 Associates:** Professional, well-equipped, prefer negotiation to violence

### Possible Approaches

#### Negotiation
- Split the goods among all parties
- Work together against outside threats
- Make deals for future cooperation
- Establish territorial agreements

#### Intimidation
- Use reputation and connections to assert authority
- Threaten consequences from allied factions
- Demonstrate superior numbers or equipment

#### Deception
- Misdirection about cache contents or value
- False information about law enforcement
- Hidden agendas and secret alliances

#### Combat
- Last resort if negotiations completely fail
- Environmental hazards make fighting dangerous
- Focus on escape rather than victory

### Complications
- **Tide Coming In:** Limited time before basement floods
- **Granny Might Call Guards:** Loud activity draws attention
- **Structural Damage:** Fighting could collapse floors
- **Cache Weight:** Goods are heavy and awkward to move quickly

\columnbreak

### Key Roleplay Moments
- **Sal's Professional Approach vs. Rusty's Desperation:** Creates natural tension
- **Moral Choices:** Violence vs. cooperation, greed vs. community impact
- **Species Dynamics:** How different cultural approaches affect negotiations
- **Community Considerations:** Impact on neighborhood and residents

<div class='note'>

#### <u>Managing the Three-Way Conflict</u>

**Sal's Priorities:** Recover goods for family honor, avoid unnecessary violence, maintain professional reputation

**Rusty's Priorities:** Get enough money to escape debts, willing to fight desperately, has nothing left to lose

**Character Options:** Can ally with either party, broker deals between them, or try to claim everything for themselves

**Crime Family Dynamics:** Remy's Whisker Family membership creates complex negotiations - Sal must respect inter-family protocols while Remy has inside knowledge of criminal operations

**Environmental Pressure:** Tidal timing forces quick decisions

</div>

<div class="footnote">THE SMUGGLER'S CACHE<BR />
<p>THE GREAT BURROW</p></div>

\pagebreakNum

## Scene 3.5: The Silverclaw Intervention
*20 minutes - Guaranteed Combat Encounter*

### Setup
Just as negotiations between characters, Sal's crew, and Rusty's group reach a critical point, **"Ripsaw" Rourke Silverclaw** and her otter enforcers arrive to claim territorial rights over the waterfront cache. Unlike the previous encounters, this scene is designed to escalate to combat due to built-in conflicts with the party.

### Why Combat is Guaranteed
- **Pine's -2 Silverclaw Reputation:** As a Ranger, Pine has actively opposed Silverclaw operations, making negotiation impossible
- **Territorial Claims:** The Silverclaws consider all Lin's Brook waterfront their domain
- **No Sharing:** Ripsaw doesn't negotiate with "land creatures" about water rights

### Participants
- **"Ripsaw" Rourke Silverclaw + 3 Otter Enforcers:** Aggressive, territorial, won't back down
- **Existing parties must choose sides or flee:** Sal's crew may join fight or withdraw; Rusty's group likely flees

### Key NPCs for This Scene

#### "Ripsaw" Rourke Silverclaw
*Silverclaw Family Lieutenant*

<div class="archetype">
<span class="bra">3</span>
<span class="agi">4</span>
<span class="int">2</span>
<span class="cun">3</span>
<span class="wil">2</span>
<span class="pre">2</span>
</div>

<div class="adversary">
<span class="soak">4</span>
<span class="wound">15</span>
<span class="strain">13</span>
<span class="mdef">1</span>
<span class="rdef">1</span>
</div>

**Skills:** Athletics 3 (**Water +3 <span class='boost'>b</span><span class='boost'>b</span><span class='boost'>b</span>**), Brawl 2, Coercion 2, Skulduggery 2, Streetwise 2, Vigilance 2, Stealth 1

**Talents:** 
- **Aquatic Excellence:** Add <span class='boost'>b</span><span class='boost'>b</span><span class='boost'>b</span> to swimming, hold breath for extended periods
- **Slippery:** Add <span class='boost'>b</span> to escape restraints and grapples
- **Pack Coordination:** Grant allies <span class='boost'>b</span> to coordinated attacks
- **Adversary 1:** Upgrade difficulty of attacks against her once

**Equipment:** Reinforced vest, jagged blade "Ripsaw" (Damage 4, Crit 2, Vicious 1), smoke grenades for escape

**Personality:** Ruthless, territorial, cunning enough to escape when outmatched
**Motivation:** Prove herself to Mother Marta by securing Silverclaw territory
**Speech Pattern:** Aggressive otter speech with violent water metaphors
**Escape Plan:** Uses smoke grenades and superior swimming to flee through waterfront when defeated

#### Silverclaw Enforcers (3)
*Otter Gang Members*

**Characteristics:** Brawn 3, Agility 2, Intellect 1, Cunning 2, Willpower 2, Presence 1

<div class="minion">
<span class="soak">3</span>
<span class="wound">4</span>
<span class="mdef">0</span>
<span class="rdef">0</span>
</div>

**Skills (Group Only):** Brawl 2, Athletics 2 (**Water +2 <span class='boost'>b</span><span class='boost'>b</span>**), Skulduggery 1

**Talents:** Aquatic (hold breath for extended periods, swim at full speed)

**Equipment:** Club weapons (Damage 4, Crit 4), protective vests

### Tactical Considerations
- **Environmental Advantages:** Otters fight better near water and in tight spaces
- **Pack Tactics:** Work together to overwhelm single targets
- **Escape Routes:** Will retreat to water if losing, potentially taking cache goods
- **Structural Damage:** Combat in deteriorating warehouse is dangerous for everyone

### Combat Triggers
- Pine's presence immediately escalates tension
- Any attempt to claim "otter territory"
- Characters showing "disrespect" to Ripsaw
- Refusing to surrender cache to "rightful claimants"

<div class='note'>

#### <u>Managing the Combat</u>

**Opening:** Ripsaw recognizes Pine as "that Ranger scum" and attacks immediately
**Tactics:** Otters use superior mobility and pack coordination
**Stakes:** Cache goods may be damaged in fighting
**Resolution:** Defeat, negotiation from position of strength, or strategic withdrawal

</div>

<div class="footnote">THE SMUGGLER'S CACHE<BR />
<p>THE GREAT BURROW</p></div>

\pagebreakNum

## Scene 4: The Law Arrives
*30 minutes - Social Encounter with Authority*

### Setup
Officer Tidecaller arrives to investigate reports of suspicious activity. How this plays out depends on previous choices and current situation.

### Variables Affecting This Scene
- **What Granny Reported:** From "suspicious activity" to "armed criminals"
- **Current Situation:** Who's present, what's visible, tension level
- **Character Reputation:** Previous interactions with law enforcement
- **Evidence of Crime:** Obvious illegal activity vs. plausible explanations

### Officer Tidecaller's Priorities
1. **Community Safety:** Protecting residents and maintaining peace
2. **Investigation:** Understanding what's really happening
3. **Law Enforcement:** Dealing with obvious criminal activity
4. **Pragmatism:** Avoiding unnecessary paperwork if possible

### Possible Approaches
- **Cooperation:** Work with officer to resolve situation legally
- **Deception:** Hide criminal activity, claim legitimate business
- **Bribery:** Offer money or favors for looking the other way
- **Escape:** Avoid confrontation entirely through stealth or misdirection

### Outcomes Depend On
- How characters present themselves and their story
- Whether violence has occurred or is threatened
- Community impact and Granny Driftwood's opinion
- Evidence of obvious criminal activity
- Characters' reputation with law enforcement

\columnbreak

<div class='example'>

##### Law Enforcement Encounter

**Cooperative Approach:** "Officer, we're investigating some stolen property for a local business. We'd be happy to coordinate with you to ensure everything's handled properly."

**Deceptive Approach:** "We're here on behalf of the property owner to assess the building for renovation. These other folks seem to be trespassing."

**Pragmatic Approach:** "Officer, there's a complicated situation here involving missing goods and competing claims. Maybe we can work together to sort this out?"

</div>

<div class="footnote">THE SMUGGLER'S CACHE<BR />
<p>THE GREAT BURROW</p></div>

\pagebreakNum

## Scene 5: The Resolution
*30 minutes - Consequences and Wrap-up*

### Setup
Based on previous choices, characters deal with the aftermath and consequences of their decisions.

### Possible Outcomes

#### Cooperative Resolution
- Characters, Sal, and possibly Rusty work out a deal
- Goods are split or sold with profits shared
- Crime family gets their cut, everyone else benefits
- Community relationships are maintained or improved
- **Reputation:** +1 with all involved parties

#### Criminal Success  
- Characters escape with some or all of the cache
- Must deal with ongoing crime family pressure
- Reputation in criminal circles improves
- Legal heat and community suspicion increase
- **Reputation:** +2 Criminal, -1 Law Enforcement, -1 Community

#### Legal Resolution
- Officer Tidecaller mediates a legal solution
- Goods are returned to proper authorities
- Characters might receive finder's fee or legal immunity
- Community standing improves, criminal contacts suffer
- **Reputation:** +2 Law Enforcement, +1 Community, -2 Criminal

\columnbreak

#### Violent Outcome
- Combat has occurred with consequences
- Injured parties need medical attention
- Legal investigation becomes serious
- Community trust is damaged
- Ongoing feuds and revenge plots
- **Reputation:** -1 to -3 with multiple factions

### Long-term Consequences
- **Reputation Changes:** Affect future opportunities and adventures
- **Economic Impact:** Money gained or lost, debts settled or incurred
- **Relationship Changes:** NPCs remember character actions
- **Future Adventure Hooks:** Established through resolution choices

<div class='note'>

#### <u>Measuring Success</u>

Success in The Smuggler's Cache isn't just about treasure gained. Consider:

**Community Impact:** How do character actions affect neighborhood stability?
**Relationship Building:** What connections are formed or destroyed?
**Problem Solving:** How creatively do characters approach challenges?
**Moral Choices:** Do characters consider broader consequences?

The "best" outcome balances personal gain with community wellbeing.

</div>

### Future Adventure Hooks
- **Crime Family Recruitment:** Sal wants to hire characters for bigger jobs
- **Law Enforcement Contact:** Officer Tidecaller asks for help with investigations
- **Business Opportunities:** Whiskers has more "import/export" work
- **Community Problems:** Granny Driftwood needs help with neighborhood issues
- **Gentrification Resistance:** Characters become involved in community organizing
- **Smuggling Network:** Larger criminal enterprises seek their skills

<div class="footnote">THE SMUGGLER'S CACHE<BR />
<p>THE GREAT BURROW</p></div>

\pagebreakNum

# GM Resources

## Quick Reference Tables

### Tidal Schedule *(For Timing Pressure)*
| Time | Tide Level | Cache Access | Urgency |
|:---:|:---|:---|:---|
| High Tide | Basement flooded | Inaccessible | 6 hours until low |
| Mid-Falling | Partially flooded | Difficult, dangerous | 3 hours until low |
| Low Tide | Basement accessible | Full access | 3 hours until rising |
| Mid-Rising | Partially flooded | Difficult, dangerous | 3 hours until high |

\columnbreak

### NPC Quick Stats
| Character | Motivation | Approach | Key Information |
|:---|:---|:---|:---|
| **Finn** | Get out of jail, retrieve cache | Nervous, helpful | Cache location, combination |
| **Whiskers** | Satisfy crime family | Professional, worried | Criminal connections, pressure |
| **Sal** | Recover goods, maintain honor | Reasonable but firm | Family operations, consequences |
| **Rusty** | Escape debts, score big | Desperate, violent | Jail gossip, nothing to lose |
| **Officer Tidecaller** | Community peace | Fair but strict | Legal authority, investigation |
| **Granny** | Protect neighborhood | Observant, protective | Recent activity, community impact |

### Economic Reference
- **Daily Wages:** 5-20 acorns depending on skill level
- **Monthly Rent:** 50-200 acorns depending on neighborhood quality
- **Cache Value:** 3,000 acorns (life-changing money for working creatures)
- **Modest Home:** 1,000 acorns purchase price
- **Luxury Item:** 50-100 acorns typical cost

<div class="footnote">THE SMUGGLER'S CACHE<BR />
<p>THE GREAT BURROW</p></div>

\pagebreakNum

## Random Complications

| <span class='dice'>d</span><span class='dice'>d</span> | Complication |
|:---:|:---|
| 2-3 | Structural collapse threatens everyone |
| 4-5 | Additional crime family members arrive |
| 6-7 | Tide comes in faster than expected |
| 8-9 | Neighborhood residents investigate noise |
| 10-11 | Cache is partially damaged by water |
| 12 | Finn escapes jail and arrives at scene |

## Treasure Distribution Guidelines

### Possible Distributions
- **Full Success:** Characters get 70-100% of cache value (2100-3000 acorns)
- **Negotiated Split:** Characters get 30-50% of cache value (900-1500 acorns)
- **Legal Resolution:** Characters get 10-20% as finder's fee (300-600 acorns)
- **Failure/Escape:** Characters get nothing but avoid legal trouble

### Non-Monetary Rewards
- **Reputation Changes:** Standing with various factions for future opportunities
- **Contacts Gained:** New relationships with NPCs for ongoing adventures
- **Information Acquired:** Knowledge about smuggling, crime families, or opportunities
- **Favors Owed:** IOUs from grateful or impressed NPCs

<div class='note'>

#### <u>Scaling for Different Groups</u>

**Fewer Players (2-3):** Reduce NPC numbers, simplify negotiations, focus on key relationships

**More Players (5-6):** Add complications, create sub-groups with different objectives, increase stakes

**Different Experience Levels:** Adjust challenge difficulty, provide more or less guidance

**Time Constraints:** Focus on key scenes, streamline exploration and investigation

</div>

<div class="footnote">THE SMUGGLER'S CACHE<BR />
<p>THE GREAT BURROW</p></div>

\pagebreakNum

## Adventure Hooks and Continuations

### Immediate Follow-Up Adventures

#### "The Longtail Job"
If characters impressed Sal, the crime family offers them a bigger operation: moving a shipment through competing family territory. Tests loyalty vs. morality when they discover the cargo includes protection racket "insurance" payments from struggling families.

#### "The Tidecaller Investigation"  
Officer Tidecaller recruits characters to help investigate corruption in the ferry system. Characters must go undercover while balancing relationships with criminal contacts and law enforcement goals.

#### "The Whiskers Connection"
McGillicuddy offers characters legitimate import/export work, but his business practices blur legal and illegal lines. Characters must decide how far they'll go for good money.

#### "Granny's Neighborhood Watch"
Granny Driftwood asks characters to help organize community resistance to gentrification. Involves union organizing, political action, and confronting the economic forces reshaping Lin's Brook.

### Long-Term Campaign Integration

#### Reputation Consequences
- **High Criminal Reputation:** Access to illegal opportunities, but increased law enforcement scrutiny
- **High Law Enforcement Reputation:** Official missions, but difficulty accessing criminal information
- **High Community Reputation:** Local support and resources, but responsibility to help with problems

#### Ongoing Relationships
- **Sal's Crime Family:** Could become patrons, employers, or enemies depending on character choices
- **Officer Tidecaller:** Potential ally for law-abiding characters or persistent problem for criminals
- **Granny Driftwood:** Community voice and source of neighborhood information

#### Economic Impact
- **Sudden Wealth:** 3,000 acorns can fund business ventures, property purchases, or major life changes
- **Debt Settlement:** Money could resolve character background obligations or create new ones
- **Investment Opportunities:** Characters might become community stakeholders with ongoing interests


<div class='example'>

##### Campaign Integration Example

Characters who successfully negotiated a three-way split of the cache and maintained good community relations might find themselves approached by other neighborhoods facing similar gentrification pressures. Their reputation as problem-solvers who consider community impact makes them ideal for adventures involving:

- Balancing development with community preservation  
- Mediating between traditional families and new economic forces
- Investigating corruption that affects working-class creatures

</div>

### Character Development Opportunities

#### Moral Growth
- **Community vs. Personal Gain:** How much individual success is worth if it hurts neighbors?
- **Law vs. Justice:** When are legal solutions inadequate for real problems?
- **Cooperation vs. Competition:** Building alliances vs. taking everything for yourself

#### Skill Development
- **Social Networks:** Contacts gained through adventure choices
- **Local Knowledge:** Lin's Brook politics and economics
- **Criminal/Legal Expertise:** Depending on resolution path chosen

#### Reputation Evolution
- **Community Leader:** Characters who prioritize neighborhood wellbeing
- **Criminal Operator:** Characters who embrace illegal opportunities
- **Independent Problem-Solver:** Characters who maintain neutrality between factions

<div class='note'>

#### <u>Success Metrics</u>

The adventure succeeds when players:
- Feel immersed in The Great Burrow's unique urban fantasy setting
- Make meaningful choices with clear consequences that affect future opportunities
- Engage with memorable NPCs who feel like real inhabitants of this world
- Experience the tension between individual success and community responsibility
- Want to continue exploring this setting and these relationships

</div>

<div class="footnote">THE SMUGGLER'S CACHE<BR />
<p>THE GREAT BURROW</p></div>

\pagebreakNum

# Optional "Off-Rails" Scenes

*Five detailed scenes for when players go off the expected path*

## Optional Scene 1: The Guild Hall Meeting
*When players need neutral ground or community backup*

### When to Use
- Players feel overwhelmed by multiple criminal threats
- Characters want to involve the community or seek protection
- Burl's union connections become relevant
- Group needs time to plan and strategize

### Location & Atmosphere
The Lin's Brook Dockworkers Guild Hall - a sturdy beaver-built structure with meeting rooms, a common area with union notices, and the lingering smell of sawdust and honest labor. Union banners hang from the rafters, and the walls are covered with photos of major construction projects.

### Key NPCs
- **Boss Ironjaw Sturgeon** (otter union leader): Gruff but fair, suspicious of criminal activity but protective of members
- **Craftsmaster Hickory Flathead** (elderly beaver): Remembers building the warehouse, knows all its secrets
- **Various Union Members**: Provide community context and working-class perspectives

### Scene Opportunities
- **Information Gathering**: Learn warehouse construction secrets and structural weaknesses
- **Community Protection**: Organize union members to "keep watch" on criminal activity
- **Neutral Negotiations**: Use guild hall as meeting place with criminal parties
- **Resources**: Access to construction equipment, tools, and local knowledge

### Complications
- Union leaders demand honesty about criminal involvement
- Some members have family connections to crime organizations
- Guild politics between species (otter vs. beaver leadership)
- Pressure to choose between individual gain and community welfare


## Optional Scene 2: Granny's Tea Service
*When players need community allies and neighborhood history*

### When to Use
- Characters need safe haven or healing after conflict
- Players want to understand gentrification impact
- Group needs an information hub about recent activity
- Moral choices about community vs. personal gain arise

### Location & Atmosphere
Granny Driftwood's cozy lodge front room, overlooking the warehouse. Handmade quilts, beaver-crafted furniture, family photos spanning decades, and the ever-present smell of bark tea. Her binoculars rest on the windowsill next to a plate of acorn cookies.

### Key NPCs
- **Granny Driftwood**: Already established, but here she becomes the community's voice
- **Neighbor Creatures**: Various Lin's Brook residents who trust Granny's judgment
- **Young Kit Visitors**: Grandchildren and neighborhood young ones who reveal community concerns

### Scene Opportunities
- **Community Intelligence**: Detailed observations of all recent warehouse activity
- **Moral Guidance**: Granny provides perspective on right vs. wrong choices
- **Safe Harbor**: Medical attention, food, and temporary shelter
- **Historical Context**: Stories about the warehouse's construction and neighborhood changes

### Complications
- Granny's help comes with expectations of honest behavior
- Neighbors might gossip about character activities
- Community obligations vs. criminal opportunities
- Generational conflict between traditional values and modern pressures

<div class="footnote">THE SMUGGLER'S CACHE<BR />
<p>THE GREAT BURROW</p></div>

\pagebreakNum

## Optional Scene 3: The Ferry Terminal Stakeout
*When players need to track movement or plan escapes*

### When to Use
- Characters want to observe criminal movements without engagement
- Escape routes by water become important
- Ferry schedules affect timing of operations
- Officer Tidecaller's patrol patterns matter

### Location & Atmosphere
The bustling Greenbank Ferry Terminal during shift change. Otters loading cargo, beavers checking schedules, workers heading home. Construction equipment creates hiding spots, and the irregular ferry service adds time pressure. The sound of water and work songs fills the air.

### Key NPCs
- **Captain Splash McWhiskers** (otter ferry captain): Knows everyone, trades gossip for small favors
- **Dock Supervisor Chunk Mudslap** (beaver): Suspicious of loiterers, but respects honest workers
- **Various Passengers**: Community members with information about neighborhood changes

### Scene Opportunities
- **Surveillance**: Watch for Sal's crew, Rusty's allies, or Silverclaw activity
- **Transportation Planning**: Learn ferry schedules and water escape routes
- **Information Trading**: Exchange small favors for gossip and local knowledge
- **Cover Stories**: Blend in with legitimate dock workers and travelers

### Complications
- Officer Tidecaller's regular patrols make surveillance risky
- Ferry delays could trap characters or let enemies escape
- Worker gossip spreads quickly through the community
- Construction hazards make the area genuinely dangerous

---

## Optional Scene 4: The Underground Connection
*When players need alternate routes or Ranger knowledge*

### When to Use
- Pine's Ranger training becomes crucial for escape routes
- Characters need to avoid street-level confrontations
- Underground movements of goods or people matter
- Storm drain systems connect to broader city infrastructure

### Location & Atmosphere
The Lin's Brook storm drain system connecting to the Great Underground. Echoing tunnels with rushing water, maintenance ladders, and the occasional rat or mole worker. Emergency lighting casts eerie shadows, and the sound of the city above filters down through grates.

### Key NPCs
- **Maintenance Mole Crew**: Great Underground workers who know all tunnel systems
- **Tunnel Rat Smugglers**: Independent operators using drains for small-scale operations
- **Ranger Contact**: Another Ranger Pine knows from patrol work

\columnbreak

### Scene Opportunities
- **Secret Movement**: Bypass street surveillance using underground routes
- **Cache Transport**: Move heavy goods without being seen
- **Intelligence Network**: Access information from underground community
- **Emergency Escape**: Last-resort routes when everything goes wrong

### Complications
- Tidal flooding makes some passages dangerous or impassable
- Silverclaw family controls some underground routes
- Getting lost in unfamiliar tunnel systems
- Underground communities have their own territorial disputes

<div class="footnote">THE SMUGGLER'S CACHE<BR />
<p>THE GREAT BURROW</p></div>

\pagebreakNum

## Optional Scene 5: The Smokehouse Summit
*When complex negotiations require neutral territory*

### When to Use
- Multiple parties need to negotiate without immediate violence
- Traditional otter customs and hospitality laws apply
- Characters want to leverage cultural protocols
- Final resolution requires all parties present

### Location & Atmosphere
An ancient otter smokehouse on the waterfront, where "old laws" of hospitality still apply. Hanging fish, aromatic smoke, carved posts telling family histories, and the understanding that violence is forbidden within its walls. Even crime families respect these traditions.

### Key NPCs
- **Elder Fishmaster Silverstream** (ancient otter): Neutral arbiter who enforces traditional hospitality
- **Cultural Witnesses**: Representatives from various species who ensure protocols are followed
- **Historical Voices**: Elders who remember when such meetings solved major disputes

### Scene Opportunities
- **Protected Negotiations**: Cultural immunity from violence during talks
- **Traditional Justice**: Appeal to older customs and inter-species cooperation
- **Final Bargaining**: All parties present their claims and reach resolution
- **Cultural Learning**: Understanding how The Great Burrow traditionally handles disputes

\columnbreak

### Complications
- Hospitality laws protect everyone equally, including enemies
- Traditional protocols move slowly, creating time pressure
- Some characters might not respect or understand cultural customs
- Breaking hospitality brings severe community consequences

<div class='note'>

#### <u>Using Optional Scenes</u>

**Flexible Integration:** These scenes can be used in any order based on character choices and story flow

**Character Specific:** Each scene plays to different character strengths - Burl (Guild Hall), Cooper (community bridge-building), Lucius (underground intel), Pine (tunnel knowledge), Willow (investigation skills), Remy (cultural food connections)

**Pacing Tools:** Use these scenes to slow down or speed up the adventure based on table energy and time constraints

**Community Focus:** Each scene reinforces the theme that individual actions affect the broader community

</div>

<div class="footnote">THE SMUGGLER'S CACHE<BR />
<p>THE GREAT BURROW</p></div>

\pagebreakNum

<style>
    #p9{ display: none;}
</style>