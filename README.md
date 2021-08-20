# RetSim
A WoW TBC Classic Retribution Paladin Simulator
## TODO
* Aura System
* Combat Logger 
** Damage logger instead of returns
* Proc System 
* Player State
  * Player Stats
  * Player Stat Modifier
* Change Event Queue to SortedSet
  * Option 1: Every event gets a reference to the queue and if the event is updated, the quque re-adds the event. 
Instead of passing around a list to collect the resulting events, the event queue itself is passed and new events are added to it with a reference to it.
  * Option 2: Two Lists (ResultinEvents and ModifiedEvents) collect all the events and updates the event queue in the end