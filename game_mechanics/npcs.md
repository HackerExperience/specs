# NPCs

An NPC (non-player character) is a element of the game that is not controlled by a player. They are usually controlled by artificial intelligence.

Within Hacker Experience, we can find four different kinds of NPCs: **Services**, **Points of Interest**, **Entities** and **Bots**.

Below is a detailed description of these NPCs.

## Services

Some NPCs might offer *services* to the player, whether he requested them or not. Here are some of them:

### Banks

Banks are responsible for securing customers data and money. You can access the Bank NPC and register an account, transfer money to another bank or view your balance.

### Missions

Missions are automatically generated and presented according to each user preferences and gameplay.

[See the Missions page for more information regarding missions.]()

### Police

You do bad things and the Police will chase you down. Every breath you take might increase your Heat.

## Points of Interest

A Point of Interest (POI) is a specific location on the World Map. It usually points to a virtual building that simulates a similar real-life building.

For instance, suppose there is a hotel on a specific street corner. The game might simulate this hotel, by instanciating a virtual building that acts as a hotel. That hotel probably will have a Wi-Fi connection that you can hack.

The purpose of POIs is twofold. First, they allow players to interact with the world surrounding them. It feels real when you are hacking the (virtual) hotel that lies on that street corner. Second, it adds targets that players can hack in case there is no one nearby.

The numbers of POIs depends on the player density of the region. A small town with one player might have a couple POIs, while Manhattan may have dozens.

A POI might also act as an entity. An example is a Police Department building that is a POI and, at the same time, an entity that holds criminal records of virtual citziens (See below).

## Entities

Entities are (virtual) players and buildings that you can interact with in a special way.

### Virtual Citzen

A Virtual Citzen (VC) is, as the name says, a virtual person that has her life simulated within the game. Virtual Citzens have names, relatives, jobs, bank accounts, phone numbers, criminal records, health records, SSN/Passport, political preferences and so on. They might own servers, companies or even countries. 

And you, the player, can hack their entire life. You can make someone a millionaire overnight, or screw with their lives. You can make them disappear, or turn them into a felon.

### Virtual Building

A Virtual Building (VB) is a POI that holds Virtual Citzens data. Common VBs include Hospital, City Hall, Prison, Court House, Police Department, Chamber of Commerce or Airports.

## Bots

Bots are servers that simulate real players. They might exist for two reasons:

- **The player wants to have a "single-player experience".** The first step to provide this feature is by implementing NPCs that can simulate real players.

- **There are no players nearby.** In order to play Hacker Experience 2, there is no need for geographically close players. However, some people might feel "isolated" or "weakened" by the fact that they have no neighbors. This scenario might be more common on smaller towns and countries around the globe.

In both cases there must be a clear sign that the (real) player is hacking a simulated player.