
## Create a new project.
```
$> mix new project_name
```

## Running a project
1. Navigate to mix project folder
2. Enter iex command;
```
$> iex -S mix
```
3. Call a method;
```
iex> Cards.hello
# or
iex> Cards.hello()
```
4. When we update the code, we need to recompile it;
```
iex> recompile
```

## Calling Methods, passing returned value
```
$> deck = Cards.create_deck
$> Cards.shuffle(deck)
$> Cards.contains?(deck, "One")
```
