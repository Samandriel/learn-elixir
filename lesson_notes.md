### List comprehension
2 Ways to do list comprehension
##### Option1
```
cards = for value <- values do
  for suit <- suits do
    "#{value} of #{suit}"
  end
end

List.flatten(cards)
```
##### Option2
```
for value <- values, suit <- suits do
  "#{value} of #{suit}"
end
```
---

### Data Types
- **List:** or Array is a collection of the same thing
```
["One", "Two", "Three"]
```
- **Tuple:** is a collection of totally different things
```
{:ok, "hello"}
```
---

### Pattern Matching
To do pattern matching, number of data on both side need to be the same number
```
$> {hand, rest_of_cards} = Cards.deal(deck, 2)
$> hand
["Ace of Clubs", "Ace of Spades"]
```
```
$> color0 = ["yellow"]
$> color0
["yellow"]

$> [color1, color2, color3] = ["red", "green", "blue"]
$>color1
"red"
```
---

### Save data File
```
def save(deck, filename) do
  binary = :erlang.term_to_binary(deck)
  File.write(filename, binary)
end
```
