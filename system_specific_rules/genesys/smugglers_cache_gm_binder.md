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

</style>


# The Smuggler's Cache
*A One-Shot Adventure for The Great Burrow*

In the gentrifying waterfront district of Lin's Brook, a hidden cache of valuable contraband has drawn the attention of multiple parties. What starts as a simple treasure hunt becomes a complex web of competing interests, moral choices, and the gray areas between legal and illegal that define life in the forest metropolis.

     This adventure tests characters' ability to navigate urban politics, species relationships, and the delicate balance between community and profit that shapes daily life in The Great Burrow. Success isn't just about claiming treasure - it's about understanding the consequences of choices in a city where everyone's connected to someone.

<div class="footnote">THE SMUGGLER'S CACHE<BR />
<p>THE GREAT BURROW</p></div>

\pagebreakNum

# Adventure Overview

## Setup Information

**Duration:** 3-4 hours  
**Players:** 3-5 characters  
**Tone:** Urban exploration with social intrigue and action  
**Themes:** Competing interests, moral choices, urban survival, species cooperation

### The Central Hook

While exploring an abandoned warehouse in the Greenbank district of Lin's Brook, the characters discover a hidden cache of valuable contraband. However, they're not the only ones looking for it - crime family enforcers and desperate smugglers are also converging on the location, all while trying to avoid the attention of burrow guards who would arrest everyone involved.

### The Stakes

- **Personal:** The cache contains 1,400 acorns worth of goods - enough to solve immediate financial problems
- **Social:** Getting caught could ruin reputations and relationships across burrows
- **Political:** The contraband reveals corruption in the ferry system and trade regulations
- **Community:** How the situation resolves affects ongoing gentrification and working-class displacement

### Adventure Structure

The adventure unfolds through five key scenes, each building tension while offering multiple resolution paths:

1. **The Discovery** - Characters find the cache location
2. **The Watchers** - Local resident involvement and information gathering
3. **The Competition Arrives** - Three-way confrontation with competing parties
4. **The Law Arrives** - Authority involvement based on previous choices
5. **The Resolution** - Consequences and follow-up opportunities

\columnbreak

<div class='note'>

#### <u>Running This Adventure</u>

**Flexible Beginning:** Characters can discover the cache through multiple means - accidental exploration, hired investigation, tip from informants, or following suspicious activity.

**Multiple Solutions:** Every scene has several resolution paths. Encourage creative problem-solving and negotiation over combat.

**Consequences Matter:** Choices affect reputation with different factions and create opportunities for future adventures.

**Urban Focus:** This is a city adventure - emphasize the interconnected nature of the community and how actions ripple outward.

</div>

## Background Information

### The Smuggling Operation

Three months ago, **Finn Shellcracker** (otter ferry operator) was running a small smuggling operation, moving luxury goods from Mousehattan to Scurry Island without paying proper tariffs. His contact was **Whiskers McGillicuddy** (mouse "import/export specialist") who had connections with the Longtail crime family.

When a burrow guard investigation got too close, Finn panicked and hid his most valuable shipment in an abandoned warehouse, planning to retrieve it once things cooled down.

### The Complication

Finn was arrested two weeks ago on unrelated charges (drunk and disorderly during an otter slide race). In jail, he let slip details about the cache to his cellmate **Rusty Crowbar** (rat small-time criminal). Rusty has since been released and is planning to steal the cache.

Meanwhile, Whiskers has been pressuring the Longtail family to find the missing goods, leading to **Salvatore "Sal" Longtail** (rat crime family enforcer) being assigned to recover the shipment.

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

**Talents:** Aquatic Mastery (add <span class='boost'>b</span><span class='boost'>b</span> to Athletics in water), Playful Nature (add <span class='boost'>b</span> to Charm, remove <span class='setback'>b</span> from social), Slippery (add <span class='boost'>b</span> to escape restraints), Toughened (WT +2)

**Equipment:** Reinforced vest, diving suit, rope, emergency rations, waterproof message tube

**Personality:** Nervous, talkative, tries to be helpful but makes things worse  
**Motivation:** Get out of jail and retrieve his cache without getting killed  
**Speech Pattern:** Fluid otter speech with dock worker slang and water metaphors  
**Current Status:** In Lin's Brook jail, available for questioning if characters visit

<div class="read">

*A sleek brown otter sits hunched on the jail's stone bench, his usually glossy fur dulled and unkempt. His webbed paws fidget constantly, and his dark eyes dart nervously between you and the cell door. When he speaks, his voice carries the fluid cadence of his species but trembles with anxiety.*

"Listen, I can explain everything - well, most of it anyway. This whole mess just got away from me like a riptide, you know? One minute I'm running a simple side business, next thing the current's pulling me under and I'm sitting here while my whole life's work is hidden where the tide can't reach it. You seem like reasonable folk - maybe we can help each other navigate these choppy waters?"

</div>

\columnbreak

**Key Information Finn Provides:**
- Exact location of the cache in the warehouse basement
- Combination to the lock (his daughter's birthday)
- Contents: honey liqueur, silk scarves, rare spices, luxury goods
- Warning about tidal timing - cache only accessible at low tide
- Mentions both Whiskers and "that crazy rat" (Rusty) as potential problems

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

**Talents:** Tunnel Sense (remove <span class='setback'>b</span> from underground Navigation), Precise Work (add <span class='boost'>b</span> to Mechanics), Social Networks (additional Mousehattan contact), Grit (ST +1)

**Equipment:** Work clothes, tunnel digging kit, magnifying glass, firefly lantern, emergency rations

**Personality:** Smooth-talking, well-dressed, nervous about crime family pressure  
**Motivation:** Recover goods to satisfy Longtail family and save his reputation  
**Speech Pattern:** Precise mouse diction with business jargon  
**Location:** Mousehattan financial district, but will travel to meet characters

<div class="read">

*An impeccably groomed mouse approaches, his gray fur perfectly combed and his tiny whiskers waxed to sharp points. He wears a miniature vest of fine cloth and carries himself with the practiced confidence of old Mousehattan money, though you notice his paws shake slightly as he adjusts his spectacles. His voice is cultured and precise, each word carefully chosen.*

"Good day. I am Whiskers McGillicuddy of McGillicuddy Import & Export - perhaps you've heard of our firm? I find myself in need of... discrete assistance with a matter of some delicacy. Let's discuss this professionally, shall we? Time, as they say in the financial district, is acorns, and I'm afraid both are in rather short supply at the moment."

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

**Talents:** Adaptable (once per session add <span class='boost'>b</span> to any check), Network Builder (reduce Streetwise difficulty by 1), Survivor's Instinct (add <span class='boost'>b</span> to Vigilance and Cool), Nobody's Fool (upgrade difficulty of social checks targeting him), Sixth Sense (once per session add <span class='boost'>b</span><span class='boost'>b</span> to Vigilance/Perception)

**Equipment:** Padded jacket, concealed knife, family identification, emergency funds

**Personality:** Professional, intimidating, surprisingly reasonable if treated with respect  
**Motivation:** Recover family property, maintain reputation, avoid unnecessary violence  
**Speech Pattern:** Confident rat speech with family metaphors  
**Resources:** 2-3 rat associates, crime family backing, knowledge of underground

<div class="read">

*A large, well-built rat emerges from the shadows, his dark fur immaculately groomed and his posture radiating quiet authority. Unlike the flashy new-money rats of Mousehattan, he dresses simply but expensively - quality speaks louder than ostentation. His tail, longer than most, moves with deliberate control, and his dark eyes assess you with professional interest rather than hostility.*

"Good evening. I am Salvatore Longtail, and I represent certain... family interests in this matter. I understand there may be some confusion about ownership of certain goods. Nothing personal, you understand - just business. Perhaps we can resolve this like civilized creatures? The family appreciates cooperation, and we remember our friends."

</div>

\columnbreak

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

**Talents:** Basic criminal abilities, no special training

**Equipment:** Makeshift crowbar weapon (Damage 3, Crit 4), ragged clothes, stolen goods

**Personality:** Desperate, paranoid, quick to violence when cornered  
**Motivation:** Score big to pay off debts and get out of the city  
**Speech Pattern:** Street rat slang, nervous energy  
**Resources:** Improvised weapons, knowledge of abandoned buildings, nothing to lose

<div class="read">

*A scrawny rat with patchy fur and wild eyes skulks into view, clutching a makeshift weapon - a sharpened piece of metal that might once have been a crowbar. His clothes are mismatched and dirty, and he moves with the twitchy energy of someone who's been looking over his shoulder for too long. Scars crisscross his arms and face, telling stories of a hard life in the city's underbelly.*

"Well, well, what do we got here? More treasure hunters, eh? Listen up, this is MY score, see? Been planning this for weeks, and I ain't letting nobody muscle in on my ticket out of this rat-hole city. You seem like smart folk - walk away now and nobody gets hurt. This is my one shot at the big time, and I ain't going back to scraping for scraps!"

</div>

<div class="footnote">THE SMUGGLER'S CACHE<BR />
<p>THE GREAT BURROW</p></div>

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

**Talents:** Aquatic Mastery, Playful Nature, Natural Leader, Law Enforcement Training

**Equipment:** Guard uniform with badge, official weapon, restraints, communication device

**Personality:** Dedicated, fair but strict, knows the neighborhood well  
**Motivation:** Keep the peace, investigate suspicious activity, protect community  
**Speech Pattern:** Authoritative otter speech with water metaphors  
**Resources:** Legal authority, backup guards, knowledge of local crime

<div class="read">

*A sturdy otter in the blue-gray uniform of the Lin's Brook Guard approaches with confident, measured steps. Her badge gleams against her dark brown fur, and her keen eyes miss nothing as they sweep the area. She carries herself with the easy authority of someone who knows her beat intimately and takes pride in protecting it.*

"What's going on here, citizens? I've had reports of suspicious activity in this area, and I can see why. This warehouse has been empty for months, and suddenly there's more traffic than a salmon run. I know most of you by sight, but some faces are new to these waters. Mind explaining what brings you to this particular corner of my beat?"

</div>

\columnbreak

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

**Talents:** Master Builder (add <span class='boost'>b</span> to construction Mechanics), Aquatic, Sturdy (Soak +1), Neighborhood Watch

**Equipment:** Comfortable home furnishings, binoculars, tea service, emergency supplies

**Personality:** Elderly, observant, protective of neighborhood, suspicious of outsiders  
**Motivation:** Preserve community character, watch out for trouble  
**Speech Pattern:** Deliberate beaver speech with construction metaphors  
**Location:** Lives across from warehouse, watches everything from her window

<div class="read">

*An elderly beaver sits in her window, a steaming cup of bark tea in her weathered paws and a pair of well-used binoculars around her neck. Her gray-streaked fur is neatly groomed, and she wears a hand-knitted shawl that speaks of practical comfort over fashion. Her lodge is clearly well-maintained - a testament to beaver craftsmanship and pride.*

"Well now, what have we here? More strangers poking around that old warehouse, I see. In my day, creatures minded their own business and respected their neighbors' property. That building's been nothing but trouble since the lumber company moved out - bringing all sorts of unsavory types to our quiet street. You seem different from the others, though. Got an honest look about you. Care to tell an old beaver what's really going on over there?"

</div>

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

#### Basement *(Cache Location)*
- **The Hidden Cache:** Behind false wall, accessible only at low tide
- **Flooding:** Basement floods during high tide, making access dangerous
- **Contents:** 50 bottles honey liqueur, silk scarves, rare spices, luxury goods
- **Total Value:** 1,400 acorns
- **Challenges:** Tidal timing, structural damage, concealed entrance

\columnbreak

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
| Premium Honey Liqueur | 50 bottles | 10 acorns | 500 acorns |
| Silk Scarves (Hives) | 10 pieces | 20 acorns | 200 acorns |
| Rare Spices (Coastal) | 10 containers | 30 acorns | 300 acorns |
| Luxury Goods (Mousehattan) | 10 items | 40 acorns | 400 acorns |
| **Total Cache Value** | | | **1,400 acorns** |

For perspective: This is enough to buy a modest family home, represents 3-4 months wages for skilled workers, or could fund a small business startup.

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

<div class="footnote">THE SMUGGLER'S CACHE<BR />
<p>THE GREAT BURROW</p></div>

\pagebreakNum

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

## Greenbank Ferry Terminal
*Potential Escape Route*

### Description
Small dock with irregular ferry service to other parts of the city. Currently under renovation, creating both hiding spots and obstacles for characters trying to escape with goods.

### Tactical Considerations
- Multiple escape routes by water for those who can swim
- Construction equipment provides cover during confrontations
- Ferry schedules affect timing - may not be available when needed
- Officer Tidecaller patrols here regularly

\columnbreak

<div class='note'>

#### <u>Using Locations Effectively</u>

**The Warehouse** serves as the central location but shouldn't confine the entire adventure. Let characters explore the neighborhood.

**Granny's House** provides crucial exposition and shows community impact. Her reaction to events affects the adventure's tone.

**Optional Locations** add depth and give characters choices about how to approach problems. Not every location needs to be visited.

**Environmental Storytelling** - Each location should reinforce themes of gentrification, community change, and the tension between old and new ways of life.

</div>

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

### Resolution
Characters should end this scene with knowledge of the cache location and an understanding that they're not alone in their interest. The scene sets up the social dynamics that will drive the rest of the adventure.

<div class='example'>

##### Discovery in Action

"You notice fresh scratches around the basement door - someone's been working on the lock recently. The dust patterns on the stairs show at least three different sets of prints: large ones that might be rat, smaller precise ones that could be mouse, and your own. Through the broken windows, you can see an elderly beaver across the street watching your every move with obvious interest."

</div>

\columnbreak

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
- **Rusty Crowbar:** Desperate, armed with improvised weapons, fighting alone
- **Sal + 2 Associates:** Professional, well-equipped, prefer negotiation to violence

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

**Environmental Pressure:** Tidal timing forces quick decisions

</div>

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

<div class="footnote">THE SMUGGLER'S CACHE<BR />
<p>THE GREAT BURROW</p></div>

\pagebreakNum

### Outcomes Depend On
- How characters present themselves and their story
- Whether violence has occurred or is threatened
- Community impact and Granny Driftwood's opinion
- Evidence of obvious criminal activity
- Characters' reputation with law enforcement

<div class='example'>

##### Law Enforcement Encounter

**Cooperative Approach:** "Officer, we're investigating some stolen property for a local business. We'd be happy to coordinate with you to ensure everything's handled properly."

**Deceptive Approach:** "We're here on behalf of the property owner to assess the building for renovation. These other folks seem to be trespassing."

**Pragmatic Approach:** "Officer, there's a complicated situation here involving missing goods and competing claims. Maybe we can work together to sort this out?"

</div>

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
- **Cache Value:** 1,400 acorns (life-changing money for working creatures)
- **Modest Home:** 1,000 acorns purchase price
- **Luxury Item:** 50-100 acorns typical cost

\columnbreak

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
- **Full Success:** Characters get 70-100% of cache value (980-1400 acorns)
- **Negotiated Split:** Characters get 30-50% of cache value (420-700 acorns)
- **Legal Resolution:** Characters get 10-20% as finder's fee (140-280 acorns)
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
- **Sudden Wealth:** 1,400 acorns can fund business ventures, property purchases, or major life changes
- **Debt Settlement:** Money could resolve character background obligations or create new ones
- **Investment Opportunities:** Characters might become community stakeholders with ongoing interests

\columnbreak

<div class='example'>

##### Campaign Integration Example

Characters who successfully negotiated a three-way split of the cache and maintained good community relations might find themselves approached by other neighborhoods facing similar gentrification pressures. Their reputation as problem-solvers who consider community impact makes them ideal for adventures involving:

- Union organizing and labor disputes
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
- **Local Knowledge:** Understanding Lin's Brook politics and economics
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

<style>
    #p9{ display: none;}
</style>