## 1.

**Poved:** Whales are mammals.

**Referenčna formula (GT):**

```
∀x (Whale(x) → Mammal(x))
```

**gpt_oss_20b · metoda A:**

```
∀x (Whale(x) → Mammal(x))
```

**llama3.1 · metoda A:**

```
Mammal(whale)
```

**gpt_oss_20b · metoda B:**

```
∀x (Whale(x) → Mammal(x))
```

**llama3.1 · metoda B:**

```
∀x (Whale(x) → Mammal(x))
```

## 2.

**Poved:** Mountains are tall.

**Referenčna formula (GT):**

```
∀x (Mountain(x) → Tall(x))
```

**gpt_oss_20b · metoda A:**

```
∀x (Mountain(x) → Tall(x))
```

**llama3.1 · metoda A:**

```
∀x (Mountain(x) → Tall(x))
```

**gpt_oss_20b · metoda B:**

```
∀x (Mountain(x) → Tall(x))
```

**llama3.1 · metoda B:**

```
∀x Mountain(x) → Tall(x)
```

## 3.

**Poved:** Tomatoes are red.

**Referenčna formula (GT):**

```
∀x (Tomato(x) → Red(x))
```

**gpt_oss_20b · metoda A:**

```
∀x (Tomato(x) → Red(x))
```

**llama3.1 · metoda A:**

```
∀x (Tomato(x) → Red(x))
```

**gpt_oss_20b · metoda B:**

```
∀x (Tomato(x) → Red(x))
```

**llama3.1 · metoda B:**

```
∀x Tomato(x) → Red(x)
```

## 4.

**Poved:** Dogs are domesticated mammals.

**Referenčna formula (GT):**

```
∀x (Dog(x) → (Domesticated(x) ∧ Mammal(x)))
```

**gpt_oss_20b · metoda A:**

```
∀x (Dog(x) → (Mammal(x) ∧ Domesticated(x)))
```

**llama3.1 · metoda A:**

```
∀x (Dog(x) → Domesticated(x)) ∧ Mammal(x)
```

**gpt_oss_20b · metoda B:**

```
∀x (Dog(x) → (Mammal(x) ∧ Domesticated(x)))
```

**llama3.1 · metoda B:**

```
∀x ((Dog(x) ∧ Mammal(x)) → Domesticated(x))
```

## 5.

**Poved:** Dolphins are mammals and can swim.

**Referenčna formula (GT):**

```
∀x (Dolphin(x) → (Mammal(x) ∧ CanSwim(x)))
```

**gpt_oss_20b · metoda A:**

```
∀x (Dolphin(x) → (Mammal(x) ∧ CanSwim(x)))
```

**llama3.1 · metoda A:**

```
Mammal(dolphin) ∧ CanSwim(dolphin)
```

**gpt_oss_20b · metoda B:**

```
∀x (Dolphin(x) → Mammal(x)) ∧ ∀x (Dolphin(x) → Swim(x))
```

**llama3.1 · metoda B:**

```
∀x (Mammal(x) ∧ Dolphin(x) → Swim(x))
```

## 6.

**Poved:** If a number is even, it is not odd.

**Referenčna formula (GT):**

```
∀x (Even(x) → ¬Odd(x))
```

**gpt_oss_20b · metoda A:**

```
∀x (Even(x) → ¬Odd(x))
```

**llama3.1 · metoda A:**

```
∀x (∃y EvenNumber(y) ∧ x = y → ¬OddNumber(x))
```

**gpt_oss_20b · metoda B:**

```
∀x (Even(x) → ¬Odd(x))
```

**llama3.1 · metoda B:**

```
∀x (∃y (Even(y) ∧ y = x) → ¬ ∃z (Odd(z) ∧ z = x))
```

## 7.

**Poved:** If a vehicle is a truck, it is not a car.

**Referenčna formula (GT):**

```
∀x (Truck(x) → ¬Car(x))
```

**gpt_oss_20b · metoda A:**

```
∀x (Truck(x) → ¬Car(x))
```

**llama3.1 · metoda A:**

```
Vehicle(x) ∧ IsTruck(x) → ¬IsCar(x)
```

**gpt_oss_20b · metoda B:**

```
∀x (Vehicle(x) ∧ Truck(x) → ¬Car(x))
```

**llama3.1 · metoda B:**

```
∀x (Vehicle(x) ∧ Truck(x) → ¬Car(x))
```

## 8.

**Poved:** If a door is closed, it is not open.

**Referenčna formula (GT):**

```
∀x (Door(x) ∧ Closed(x) → ¬Open(x))
```

**gpt_oss_20b · metoda A:**

```
∀x (Closed(x) → ¬Open(x))
```

**llama3.1 · metoda A:**

```
∀x (ClosedDoor(x) → ¬Open(x))
```

**gpt_oss_20b · metoda B:**

```
∀x (Door(x) ∧ Closed(x) → ¬Open(x))
```

**llama3.1 · metoda B:**

```
∀x (Door(x) → (Closed(x) ∧ ¬Open(x)))
```

## 9.

**Poved:** If a fruit is ripe, it is not green.

**Referenčna formula (GT):**

```
∀x (Fruit(x) ∧ Ripe(x) → ¬Green(x))
```

**gpt_oss_20b · metoda A:**

```
∀x (Fruit(x) ∧ Ripe(x) → ¬Green(x))
```

**llama3.1 · metoda A:**

```
∀x (∃y (Fruit(y) ∧ Ripe(x) ∧ Has(x, y)) → ¬Green(x))
```

**gpt_oss_20b · metoda B:**

```
∀x (Fruit(x) ∧ Ripe(x) → ¬Green(x))
```

**llama3.1 · metoda B:**

```
∀x (Ripe(x) → ¬Green(x))
```

## 10.

**Poved:** When a flower is blooming, it is not wilting.

**Referenčna formula (GT):**

```
∀x (Flower(x) ∧ Blooming(x) → ¬Wilting(x))
```

**gpt_oss_20b · metoda A:**

```
∀x ((Flower(x) ∧ Blooming(x)) → ¬Wilting(x))
```

**llama3.1 · metoda A:**

```
∀x (∃y (Flower(y) ∧ Blooming(y)) → ¬Wilt(y))
```

**gpt_oss_20b · metoda B:**

```
∀x (Flower(x) ∧ Blooming(x) → ¬Wilting(x))
```

**llama3.1 · metoda B:**

```
∀x (Blooming(x) → ¬Wilting(x))
```

## 11.

**Poved:** A dessert is sweet if it has sugar or honey as an ingredient.

**Referenčna formula (GT):**

```
∀x (Dessert(x) ∧ (HasSugar(x) ∨ HasHoney(x)) → Sweet(x))
```

**gpt_oss_20b · metoda A:**

```
∀x (Sweet(x) ↔ (Dessert(x) ∧ (HasIngredient(x, sugar) ∨ HasIngredient(x, honey))))
```

**llama3.1 · metoda A:**

```
∀x (∃y (∃z (Dessert(y) ∧ Ingredient(z, y)) → Sweet(x)) ↔ (∃z (Sugar(z) ∧ Ingredient(z, x)) ∨ ∃z (Honey(z) ∧ Ingredient(z, x))))
```

**gpt_oss_20b · metoda B:**

```
∀x (Dessert(x) → Sweet(x) ↔ (Has(x, sugar) ∨ Has(x, honey)))
```

**llama3.1 · metoda B:**

```
∀x (Sweet(x) ↔ Dessert(x) ∧ (Sugar(x) ∨ Honey(x)))
```

## 12.

**Poved:** A dog is considered friendly if it doesn't bite or growl.

**Referenčna formula (GT):**

```
∀x (Dog(x) ∧ ¬(Bites(x) ∨ Growls(x)) → Friendly(x))
```

**gpt_oss_20b · metoda A:**

```
∀x (Friendly(x) ↔ (Dog(x) ∧ ((¬Bite(x)) ∨ (¬Growl(x)))))
```

**llama3.1 · metoda A:**

```
∀x (Friendly(x) ↔ (Dog(x) ∧ ¬Bites(x) ∧ ¬Growls(x)))
```

**gpt_oss_20b · metoda B:**

```
∀x (Friendly(x) ↔ (Dog(x) ∧ (¬Bite(x) ∨ ¬Growl(x))))
```

**llama3.1 · metoda B:**

```
∀x (Friendly(x) ↔ ¬(Dog(x) ∧ (∃y Bites(x, y) ∨ ∃y Grows(x, y))))
```

## 13.

**Poved:** If a person is kind and honest, they are considered a good person.

**Referenčna formula (GT):**

```
∀x (Person(x) ∧ Kind(x) ∧ Honest(x) → GoodPerson(x))
```

**gpt_oss_20b · metoda A:**

```
∀x ((Person(x) ∧ Kind(x) ∧ Honest(x)) → GoodPerson(x))
```

**llama3.1 · metoda A:**

```
∀x (∃y Person(y) ∧ Kind(x) ∧ Honest(x) → GoodPerson(x))
```

**gpt_oss_20b · metoda B:**

```
∀x ((Person(x) ∧ Kind(x) ∧ Honest(x)) → Good(x))
```

**llama3.1 · metoda B:**

```
∀x (∃y Person(y) ∧ Kind(y) ∧ Honest(y) → GoodPerson(x))
```

## 14.

**Poved:** A star is classified as a red giant when it expands and cools.

**Referenčna formula (GT):**

```
∀x (Star(x) ∧ Expands(x) ∧ Cools(x) → RedGiant(x))
```

**gpt_oss_20b · metoda A:**

```
∀x (RedGiant(x) ↔ (Star(x) ∧ Expands(x) ∧ Cools(x)))
```

**llama3.1 · metoda A:**

```
∀x (RedGiant(x) ↔ (Star(x) ∧ Expands(x) ∧ Cools(x)))
```

**gpt_oss_20b · metoda B:**

```
∀x (RedGiant(x) ↔ (Star(x) ∧ Expands(x) ∧ Cools(x)))
```

**llama3.1 · metoda B:**

```
∀x (Star(x) ∧ Classifies(RedGiant, x) ↔ (Red(x) ∧ Giant(x)))
```

## 15.

**Poved:** A country is wealthy if it has a high GDP.

**Referenčna formula (GT):**

```
∀x (Country(x) ∧ HighGDP(x) → Wealthy(x))
```

**gpt_oss_20b · metoda A:**

```
∀x (Wealthy(x) ↔ (Country(x) ∧ HighGDP(x)))
```

**llama3.1 · metoda A:**

```
WealthyCountry(x) ↔ (Country(x) ∧ HighGDP(x))
```

**gpt_oss_20b · metoda B:**

```
∀x (Wealthy(x) ↔ (Country(x) ∧ HighGDP(x)))
```

**llama3.1 · metoda B:**

```
∀x (Wealthy(x) ↔ Country(x) ∧ HighGdp(x))
```

## 16.

**Poved:** A bird is considered flightless if it lacks the ability to fly.

**Referenčna formula (GT):**

```
∀x (Bird(x) ∧ ¬CanFly(x) → Flightless(x))
```

**gpt_oss_20b · metoda A:**

```
∀x (Flightless(x) ↔ (Bird(x) ∧ ¬CanFly(x)))
```

**llama3.1 · metoda A:**

```
∀x (Flightless(x) ↔ (Bird(x) ∧ ¬CanFly(x)))
```

**gpt_oss_20b · metoda B:**

```
∀x (Flightless(x) ↔ (Bird(x) ∧ ¬CanFly(x)))
```

**llama3.1 · metoda B:**

```
∀x (Flightless(x) ↔ Bird(x) ∧ ¬Flyable(x))
```

## 17.

**Poved:** If a bird is not a penguin, it can fly, and it lays eggs.

**Referenčna formula (GT):**

```
∀x (Bird(x) ∧ ¬Penguin(x) → (CanFly(x) ∧ LaysEggs(x)))
```

**gpt_oss_20b · metoda A:**

```
∀x ((Bird(x) ∧ ¬Penguin(x)) → (CanFly(x) ∧ LaysEggs(x)))
```

**llama3.1 · metoda A:**

```
∀x (∼Penguin(x) → (CanFly(x) ∧ LaysEggs(x)))
```

**gpt_oss_20b · metoda B:**

```
∀x (Bird(x) ∧ ¬Penguin(x) → (Fly(x) ∧ LayEggs(x)))
```

**llama3.1 · metoda B:**

```
∀x (Bird(x) ∧ ¬Penguin(x) → (CanFly(x) ∧ LaysEggs(x)))
```

## 18.

**Poved:** A mammal has hair or fur.

**Referenčna formula (GT):**

```
∀x (Mammal(x) → (Hair(x) ∨ Fur(x)))
```

**gpt_oss_20b · metoda A:**

```
∀x (Mammal(x) → (Hair(x) ∨ Fur(x)))
```

**llama3.1 · metoda A:**

```
∀x (Mammal(x) → (∃y (Hair(y) ∧ Has(x, y)) ∨ ∃z (Fur(z) ∧ Has(x, z))))
```

**gpt_oss_20b · metoda B:**

```
∀x (Mammal(x) → (Hair(x) ∨ Fur(x)))
```

**llama3.1 · metoda B:**

```
∀x (Mammal(x) → (Hair(x) ∨ Fur(x)))
```

## 19.

**Poved:** A fruit can be sweet or sour.

**Referenčna formula (GT):**

```
∀x (Fruit(x) → (Sweet(x) ∨ Sour(x)))
```

**gpt_oss_20b · metoda A:**

```
∀x (Fruit(x) → (Sweet(x) ∨ Sour(x)))
```

**llama3.1 · metoda A:**

```
Fruit(x) ∧ (∃y (Sweet(y) ∧ SameFruit(x, y)) ∨ ∃z (Sour(z) ∧ SameFruit(x, z)))
```

**gpt_oss_20b · metoda B:**

```
∀x (Fruit(x) → (Sweet(x) ∨ Sour(x)))
```

**llama3.1 · metoda B:**

```
∃x (∃y Fruit(y) ∧ (Sweet(y) ∨ Sour(y)))
```

## 20.

**Poved:** A movie can be a comedy, a drama, or a thriller.

**Referenčna formula (GT):**

```
∀x (Movie(x) → (Comedy(x) ∨ Drama(x) ∨ Thriller(x)))
```

**gpt_oss_20b · metoda A:**

```
∀x (Movie(x) → (Comedy(x) ∨ Drama(x) ∨ Thriller(x)))
```

**llama3.1 · metoda A:**

```
∀x (∃y (Movie(y)) → (Comedy(x) ∨ Drama(x) ∨ Thriller(x)))
```

**gpt_oss_20b · metoda B:**

```
∀x (Movie(x) → (Comedy(x) ∨ Drama(x) ∨ Thriller(x)))
```

**llama3.1 · metoda B:**

```
∀x (Movie(x) → (Comedy(x) ∨ Drama(x) ∨ Thriller(x)))
```

## 21.

**Poved:** A switch is on or off, never both.

**Referenčna formula (GT):**

```
∀x (Switch(x) → (On(x) ⊕ Off(x)))
```

**gpt_oss_20b · metoda A:**

```
∀x (Switch(x) → ((On(x) ∨ Off(x)) ∧ ¬(On(x) ∧ Off(x))))
```

**llama3.1 · metoda A:**

```
∀x (Switch(x) → (On(x) ∨ Off(x)) ∧ ¬(On(x) ∧ Off(x)))
```

**gpt_oss_20b · metoda B:**

```
∀x (Switch(x) → ((On(x) ∨ Off(x)) ∧ ¬(On(x) ∧ Off(x))))
```

**llama3.1 · metoda B:**

```
∀x (Switch(x) → (∃y (State(y) ∧ On(y, x)) ∨ ∃z (State(z) ∧ Off(z, x))))
```

## 22.

**Poved:** A job is either part-time or full-time, but not both.

**Referenčna formula (GT):**

```
∀x (Job(x) → (PartTime(x) ⊕ FullTime(x)))
```

**gpt_oss_20b · metoda A:**

```
∀x (Job(x) ↔ ((PartTime(x) ∨ FullTime(x)) ∧ ¬(PartTime(x) ∧ FullTime(x))))
```

**llama3.1 · metoda A:**

```
∀x (∃y (PartTime(y) ∧ HasJob(x, y)) ⊕ ∃z (FullTime(z) ∧ HasJob(x, z)))
```

**gpt_oss_20b · metoda B:**

```
∀x (Job(x) → ((PartTime(x) ∨ FullTime(x)) ∧ ¬(PartTime(x) ∧ FullTime(x))))
```

**llama3.1 · metoda B:**

```
∀x (Job(x) → (∃y Is(x, y) ∧ PartTime(y) ∨ ∃y Is(x, y) ∧ FullTime(y) ∧ ¬(∃z Is(x, z) ∧ PartTime(z) ∧ FullTime(z))))
```

## 23.

**Poved:** A book can be either fiction or nonfiction, but not a mix of both.

**Referenčna formula (GT):**

```
∀x (Book(x) → (Fiction(x) ⊕ Nonfiction(x)))
```

**gpt_oss_20b · metoda A:**

```
∀x (Book(x) → ((Fiction(x) ∨ Nonfiction(x)) ∧ ¬(Fiction(x) ∧ Nonfiction(x))))
```

**llama3.1 · metoda A:**

```
∀x (Book(x) → (∃y Fiction(y) ∧ x = y ∨ ∃y NonFiction(y) ∧ x = y))
```

**gpt_oss_20b · metoda B:**

```
∀x (Book(x) → ((Fiction(x) ∨ Nonfiction(x)) ∧ ¬(Fiction(x) ∧ Nonfiction(x))))
```

**llama3.1 · metoda B:**

```
∀x (Book(x) → (∃y Fiction(y) ∧ HasContent(x, y)) ∨ (∃z Nonfiction(z) ∧ HasContent(x, z)))
```

## 24.

**Poved:** A fruit is either ripe or unripe, but not both at the same time.

**Referenčna formula (GT):**

```
∀x (Fruit(x) → (Ripe(x) ⊕ Unripe(x)))
```

**gpt_oss_20b · metoda A:**

```
∀x (Fruit(x) → (Ripe(x) ⊕ Unripe(x)))
```

**llama3.1 · metoda A:**

```
∀x (Fruit(x) → (∃y Ripe(y) ∧ Unripe(y)) ⊕ (Ripeness(x) ∧ ∃y (Ripe(y) ∧ Ripe(x)))
```

**gpt_oss_20b · metoda B:**

```
∀x (Fruit(x) → ((Ripe(x) ∨ Unripe(x)) ∧ ¬(Ripe(x) ∧ Unripe(x))))
```

**llama3.1 · metoda B:**

```
∀x (Fruit(x) → (∃y Ripe(y) ∧ ∃z Unripe(z)))
```

## 25.

**Poved:** Lions are carnivores but not all carnivores are lions.

**Referenčna formula (GT):**

```
∀x (Lion(x) → Carnivore(x)) ∧ ∃y (Carnivore(y) ∧ ¬Lion(y))
```

**gpt_oss_20b · metoda A:**

```
∀x (Lion(x) → Carnivore(x)) ∧ ∃y (Carnivore(y) ∧ ¬Lion(y))
```

**llama3.1 · metoda A:**

```
∀x (Lion(x) → Carnivore(x)) 
∧ ¬ ∀x (Carnivore(x) → Lion(x))
```

**gpt_oss_20b · metoda B:**

```
∀x (Lion(x) → Carnivore(x)) ∧ ∃x (Carnivore(x) ∧ ¬Lion(x))
```

**llama3.1 · metoda B:**

```
∀x ∀y (Lion(x) ∧ Carnivore(y) → (x = y ∧ Are(x, y)))
```
