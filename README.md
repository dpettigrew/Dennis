# Dennis
Swift Language Style Guide, Best Practices and Recommendations, and very much a work in progress.

---

DENNIS:  You're fooling yourself.  We're living in a dictatorship.
      A self-perpetuating autocracy in which the working classes--

WOMAN:  Oh there you go, bringing class into it again.

---

## Contributions

The following critiera will be used to accept contributions:

* Does the contribution solve a problem?
* Does it correct an issue in the software?
* Was it contributed to the most relevant project?
* Does it adhere to this guide (as it exists at the time of the contribution)?
* Does the contribution contain unit or functional tests?
* Does it break existing code or mitigate that breakage somehow?
* ... more to follow
 
The above being said, we want to help you meet the criteria that we've set out if your contribution doesn't already.  We'll do that through PRs, issues, carrier pidgeons, etc.

## New Projects

### Naming

New projects must have a "Monty Python and The Holy Grail" related name (whether that's a character, a place, something one might've found in said time period, whatever, it's pretty loose), in addition to a meaningful name.

Example: Soothsayer (movie reference) and THGReachability (meaningful name).  The idea being along the lines of...
```
SIR GALAHAD: Tell me soothsayer, what say you about network connectivity?
SOOTHSAYER: What connectivity?
```

The meaningful name is important as well.  Can you imagine doing this...

```Swift
import Foundation
import Soothsayer // What the hell does this do???
```

whereas...

```Swift
import Foundation
import THGReachability
```

Ah yes.  I can get an idea of what THGReachability is.

### Prefixes

Prefix only the module name, not the classes within the module.

```
RANDOM PEASANT:  Ye ole Swift guide said you don't need prefixes!
GOD:  There's 4 Swift Reachability implementations by 4 different authors that are all have the same module name, 'Reachability'.  It's like those miserable Psalms-- they're so depressing.
```
So... we will prefix our module names with THG to avoid this confusion and potential collision.  The contained enums/classes/structs shall not contain any prefixes.

Example:

THGReachability <- Module name.
Reachability <- Class inside of module.

### Project Structure
