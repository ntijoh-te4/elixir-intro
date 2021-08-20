# Elixir intro-övningar


Definera alla funktioner i modulen Intro (`lib/intro.ex`)

### Tester

Skapa tester för funktionerna i `test/intro_test.exs` **innan** du skriver funktionerna.

Försök fundera på vilka input och/eller kombinationer av input som ska generera olika output.

Exempeltest för första uppgiften:

```elixir
defmodule IntroTest do
  test "smallest of two when smallest is first" do
    assert Intro.smallest(1,2) == 1
  end

  test "smallest of two when smallest is last" do
    assert Intro.smallest(3,2) == 2
  end

  test "smallest of two of equal size" do
    assert Intro.smallest(1337,1337) == 1337
  end
end
```

Kör alla tester med `mix test`

För att manuellt testa dina funktioner med egna värden i iex, kör `iex -S mix` (observera stort "S"), och anropa sen dina tester med t.ex `Intro.smallest(3,2)`.
