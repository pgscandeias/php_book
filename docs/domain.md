# Writing Partymapper

## 2. Analysing the domain

No point in writing code before I know my domain. Let's grab a moleskine and a pen.

[Notebook picture: use cases]

There, that's my use case analysis done:

- List events happening near me
- Get details on a particular event

Not terribly complicated. Now, what kind of data model feeds these use cases?

[Notebook picture: data model]

Seems about right. `Event` is the star of the show. It belongs in a `Venue`, can be `Tag`ged with a number of categories, and may have different `Price`s - normally depending on the patron's gender and how much in advance a ticket is purchased. We don't care much about that data, but we do want to display it, so `Price` gets a catch-all `name` property to store it. `Venue`s have a location, represented by the `address` and coordinates properties... but wait, what about buildings with more than one `Venue`? I don't want overlapping pins on my map. Better make `Address` a separate entity and link it to one or more `Venue`s . Might as well make it more than a single line while we're at it, so we get nicely normalized data with separate fields for street address, door number, floor, etc. Nice.

Alright, let's get this show on the road!
