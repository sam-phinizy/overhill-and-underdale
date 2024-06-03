# Dungeons

Dungeons are the archetypal adventure location. They are dark, dangerous, and full of treasure. Dungeon implies it can be found underground but that's not always the case. They can be found in the wilderness, in the sky, or even in the ocean. They're a series of linked rooms with challenges and dangers that the party must navigate to reach the end or defeat the boss..

In Overhill & Underdale there a few different ways to adventure in a dungeon: 

- Random Pointcrawl Dungeon
- Pre-made dungeons


## Random Point Crawl Dungeon Generation

Random pointcrawl dungeons use a technique similiar to what is described on [Merkmail](https://murkdice.substack.com/p/you-liked-that-map-huh?r=3rp84v&utm_campaign=post&utm_medium=web&triedRedirect=true) to randomly generate a dungeon. It focuses on building up the 'network graph' of the dungeon rather then creating a 'concrete' map as described by Merkmail.

You can either hand draw these or use a tool like [TlDraw](https://www.tldraw.com/) to create them. The examples below use TlDraw.


### Starting a dungeon

The initial room should be labeled with a 1 as it is the entrance to the dungeon. No events happen here so you'll next determine the number of exits from the room. Roll 2d6 and consult the table below:

<a name="exits-table"></a>

| Roll | Exits |
|------|-------|
| 2    | 1     |
| 3-5  | 2     |
| 6-8  | 3     |
| 9-11 | 4     |
| 12   | 0     |

Then draw a line out from the entrance for each like this:


``` mermaid
graph LR
  1[Entrance] --- 2[Room 2]:::hidden;
  1 ---  3[Room 3]:::hidden;
  1 ---  4[Room 4]:::hidden;

  classDef hidden display: none;
```


TODO: Locked doors

Then the party should choose which door they're going through. Once you do draw another room at the end of the line and label it with the next number in the sequence. Roll on the [exits table](#exits-table) to determine how many exits the room has and repeat the process.


``` mermaid
graph LR
  1[Entrance] --- 2[Room 2];
  1 ---  3[Room 3]:::hidden;
  1 ---  4[Room 4]:::hidden;

  2 --- 5[Room 5]:::hidden;
  2 --- 6[Room 6]:::hidden;

  classDef hidden display: none;
```




