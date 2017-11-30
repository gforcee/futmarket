
## Transfers
### Current State
Below is the current state of functionality within the **Transfers** category. All methods within the Transfers category are stable. 

<img src="https://i.imgur.com/YVVgg21.png" alt="Squads" style="height: 100px;"/>

The Transfers category contains many functions. We'll go through them in three sections: Search, Transfer List, and Transfer Targets.

### Search


### fut.search()

fut.search() returns a list of dictionaries that include the information for players on the transfer market. These are returned in ascending order of seconds until expiration. just like the Web App and the console experience. [A description of the returned dict of player info is linked here.](https://github.com/TrevorMcCormick/futmarket/blob/master/lookuptables.md#player-info-dict)

```python
>>> fut.search(ctype='player', level = 'gold')
[{'assetId': 197242,
  'assists': 0,
  'attributeList': [{u'index': 0, u'value': 65},
   {u'index': 1, u'value': 58},
   {u'index': 2, u'value': 72},
   {u'index': 3, u'value': 67},
   {u'index': 4, u'value': 79},
   {u'index': 5, u'value': 86}],
  'bidState': u'none',
  ....
  ````
There are many arguments available to filter your search request:
<details>
<summary>Search Arguments Table</summary><p>
<!-- alternative placement of p shown above -->


| argument    | type    | description                                                  |
|-------------|---------|--------------------------------------------------------------|
| ctype       | str     | card type (player, development, training)                    |
| level       | str     | card level (bronze, silver, gold)                            |
| category    | str     | card category (fitness, health, etc.)                        |
| assetId     | int     | unique player id                                             |
| defId       | int     | each assetId can have multiple defIds (ex. TOTW player card) |
| min_price   | int     | minimum currentBid                                           |
| max_price   | int     | maximum currentBid                                           |
| min_buy     | int     | minimum buyNow                                               |
| max_buy     | int     | maximum buyNow                                               |
| league      | int     | leagueId (available in fut.leagues)                          |
| club        | int     | clubId (available in fut.teams)                              |
| position    | str     | player preferred position abbreviation                       |
| nationality | int     | nationalityId (available in fut.nations)                     |
| rare        | boolean | TRUE if rare card                                            |
| playStyle   | int     | playStyleId (available in fut.playStyles)                    |
| start       | int     | page to start on (indexed at 0) through the web app.         |
| page_size   | str     | cards to show on one page (range between 16-50)              |


</p></details>