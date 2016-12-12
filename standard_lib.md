# Elixir Standard Library
### Enum
##### shuffle(enumerable)
```
def shuffle(deck) do
  Enum.shuffle(deck)
end
```
##### member?()
Check if an element is a member of the list
```
def contains?(deck, card) do
  Enum.member?(deck, card)
end
```
##### split(enumerable, count)
```
Enum.split(deck, count)
```
---
### List
##### flatten()
flatten multiple list to one list
```
cards = for value <- values do
  for suit <- suits do
    "#{value} of #{suit}"
  end
end

List.flatten(cards)
```
---
### File
##### write(path, content)
Writes content to the file path.The file is created if it does not exist. If it exists, the previous contents are overwritten.
```
File.write(filename, binary) 
```
