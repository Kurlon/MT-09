# Brakes
The base 2024 MT-09 uses the same Advics radial calipers that Yamaha has used for YEARS across various bikes, particularly the 3rd Generation R6. SP models get upgraded to Brembo Stylemas. Both bikes use the same 17mm Brembo radial master and are plumbed through an ABS system.

## Pads
### Advics Calipers
EBC specs out FA252 pads for the MT-09, and doesn't offer them in their racier compounds. EBC for the R6 specs out FA380 pads, and offers them in their GPFAX compound. The pads are the same backing plate and thickness, FA252s come with anti-rattle shims, FA380s don't. Forget the FA252s exist, shop around FA380 and matching pad fitments from other providers. I'm trying DP RDP418 'RDP X-Race Titanium' pads this year on my MT-09.

Plumbed through the stock lines and ABS module, the stock 17mm Brembo master feels OK, now that I've switched to direct lines from Core Moto I'm a little worried that I'll be slightly over-mastered. On the R6 Yamaha paired these calipers with a 16mm radial master, the Advics run a slightly smaller piston area than the Stylemas. I have a couple OEM R6 masters on standby if I don't like the feel of the Brembo.

### Brembo Stylema Calipers
Haven't chased pads on these. On paper these calipers should be about 100g lighter per side than the Advics?

# Ditching Keys
Standard race prep is to get rid of anything needing a key so you don't have to worry about that on track. Unfortunately, given how few of these bikes are raced most of those parts haven't been adapted to the MT-09 yet.

## Tank
Everywhere lists the 2024+ MT-09 as working with the same keyless gas cap assemblies as the 21-23 MT-09, R6 forever, etc. This is not the case, the bolt circle is larger, and the actual tank opening is at the bottom of the bolt circle instead of the top as is normally the case on Yamahas. No keyless cap exists for these tanks yet.

## Seat
S2 Concepts out of France makes a race tail for these bikes that will let you toss the OEM seats (5lbs?!) and some of the heavy steel subframe bracketry to retain them. I've not done this upgrade yet myself.

## Ignition
Yamaha seems to be using the 2024 MT-09 to try out all sorts of new parts that don't cross to anything else. The ignition switch is one such item, unique to the 24+ MT-09 using a different connector than they ever used. No keyswitch elimination kit exists yet.

The switch uses a 6 pin, .250in wide contact connector that appears to be a 'Sumitomo' design last seen on old Kawi regulator rectifier connections. The keyswitch is a double pole single throw unit, no parking light position. SP bikes also have an immobilizer antenna to contend with. The switch jumps two circuits, one is basically an ECU 'go' trigger, the other is the main 12v feed from the batt to the rest of the harness, no relays or anything to lower the current running through the switch.

When you look at the connector, there are four wires, two thin wires, two thick wires, one of each on each side of the connector. The thin wires are the 'go' signal, thick are the power feed. Looking at the keyswitch side connector, looking into it with the locking tab facing up, the wires are:

| | locking tab | |
| --- | --- | --- |
| Blue with Black stripe | | Red |
| Orange with Blue stripe | | Blue |

Get the service manual to see the wiring diagrams for the ignition system.

### Kurlon Bypass
Remove the OEM ignition switch, this is not fun. You'll need to remove the tank and airbox, both well documented online. Then, to get the switch tower off you'll need to deal with it's four bolts. These have been installed using red or equivalent PITA loctite. I was able to remove the upper two bolts using a 6mm allen impact bit, the two lower bolts are security bolts that sheer off the heads when installed. I ended up grinding the remaining heads off, which allowed me to remove the tower and frame strengthening steel plate underneath. From there I had to use locking pliers to work the bolt stubs out. In hind sight, a torch to heat the bolts/frame up and defeat the loctite would have made things easier but I wasn't comfortable waving a torch around under there at that time.

Souce a matching connector, [Cycleterminal](https://www.cycleterminal.com/250-connectors.html) lists a Sumitomo .250 non-sealed locking connector that sounds like a match, it's locking tabs are on the wrong connector though. The harness side female connector has the lock prong, the male connector for the switch end should have a slot to recieve it, and Cycleterminal's unit flips those around. The crimp connectors they supply for it though do appear to be a close match. On the same page they list "Yazaki CN-A Locking Type - 250 Connectors" which appear to be keyed correctly and I'll be trying to get a set. If you google "sumitomo lock type 0.250 6 pin" you'll find other listings for what appear to be matching connectors, some of which come with wire leads already crimped up if you don't like crimping your own terminals.

On the new connector, wire a jumper between the Blue with Black stripe wire position and Blue wire position. This is just an ECU 'go' signal, if the switch had a park position, leaving this pair open but jumping the 12v feed would be how it would achieve that. There is no power on this loop when the 12v feed isn't connected so it won't cause a drain on the bike staying in place.

Crimp in leads to the Red and Orange with Blue stripe positions, these are what will be switched on and off to control power to the bike.

Source a suitable SPST waterproof switch, knowing it's going to see 12v DC and potentially 10A+ at times. Speedcell offers a generic 'master arm switch' kit with a suitable switch and nice 3d metal printed guard. I'll post a pic showing my setup once done.
