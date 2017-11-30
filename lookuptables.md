### Player Info Dict  
The player info dict is returned by many functions. Below is an example with a helpful table of return types.
<details>
<summary>Player Info Dict Code Example</summary><p>
<!-- alternative placement of p shown above -->

```python
>>> #Get first player in my club
>>> fut.club()[0]
[{'assetId': 230621,
  'assists': 0,
  .......}]
```
</p></details>

<details>
<summary>Player Info Dict Return Types</summary><p>
<!-- alternative placement of p shown above -->

| field             | type    | description                               |
|-------------------|---------|-------------------------------------------|
| assetId           | int     | unique asset id                           |
| assists           | int     | career assists                            |
| attributeList     | dict    | five primary stats                        |
| bidState          | str     | state of bid                              |
| buyNowPrice       | int     | coins to buy now                          |
| cardType          | int     | <font color="red">unsure</font>           |
| cardsubtypeid     | int     | <font color="red">unsure</font>           |
| contract          | int     | 0-99 games                                |
| count             | ?       | None                                      |
| currentBid        | int     | coins of currentBid (0 if no bids)        |
| discardValue      | int     | coins recieved from quick sell            |
| expires           | int     | seconds until expires from transfer market|
| fitness           | int     | 0-99 fitness                              |
| formation         | str     | current team formation                    |
| id                | int     | unique card id. one asset id can have many card ids (TOTW example) |
| injuryGames       | int     | games until current injury expires        |
| injuryType        | str     | current injury type                       |
| itemState         | str     | what you can do with the current item     |
| itemType          | str     | player, development, training             |
| lastSalePrice     | int     | coins last sold for on transfer market    |
| leagueId          | int     | use fut.leagues() to get dictionary       |
| lifetimeAssists   | int     | career assists again                      |
| lifetimeStats     | dict    | all career stats                          |
| loyaltyBonus      | int     | <font color="red">unsure</font>           |
| morale            | int     | 0-99 ... not sure what this does          |
| nation            | int     | use fut.nations() to get dictionary       |
| offers            | int     | number of bids in transfer market         |
| owners            | int     | number of historical owners               |
| pile              | int     | <font color="red">unsure</font>           |
| playStyle         | int     | use fut.playStyles() to get dictionary    |
| position          | str     | preferred player position                 |
| rareflag          | int     | rare card                                 |
| rating            | int     | 0-99                                      |
| resourceGameYear  | int     | 2018                                      |
| resourceId        | int     | same as assetid                           |
| sellerEstablished | int     | <font color="red">unsure</font>           |
| sellerId          | int     | current seller on transfer market (empty) |
| sellerName        | str     | current seller on transfer market (empty) |
| startingBid       | int     | coins of the first bid on transfer market |
| statsList         | dict    | same as lifetimeStats                     |
| suspension        | int     | red card suspension games remaining       |
| teamid            | int     | use fut.teams() to get dictionary         |
| timestamp         | int     | epoch time that you acquired the item     |
| tradeId           | int     | unique tradeId on transfer market         |
| tradeState        | str     | current State on transfer market          |
| training          | int     | <font color="red">unsure</font>           |
| untradeable       | boolean | listable on the transfer market           |
| untradeableCount  | ?       | <font color="red">unsure</font>           |
| watched           | boolean | currently in watchlist                    |
| year              | int     | 2018                                      |

  </p></details>