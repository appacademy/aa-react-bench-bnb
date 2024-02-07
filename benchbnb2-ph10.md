# BenchBnB, Phase 10: Highlighting Benches

[Live Demo]

In this final Phase, you will enhance the user experience by highlighting a
bench list item when a user hovers over its marker.

[Live Demo]: https://aa-bench-bnb.herokuapp.com/

## Highlight bench list items when hovering over markers

The final feature that you will add to your BenchBnB app--at least for now!--is
to highlight a bench list item when a user hovers over its marker.

First, add a `highlightedBench` state value to the `BenchIndexPage`. Then add
handlers to `markerEventHandlers` for `mouseover` (set `highlightedBench` to
marker's associated bench) and `mouseout` (clear `highlightedBench`).

Pass `highlightedBench` to `BenchMap` as a prop. Create a different marker style
for highlighted benches (e.g., inverted colors). Add another effect to
`BenchMap`: whenever the `highlightedBench` changes, ensure every marker whose
bench is not the `highlightedBench` has standard styling, and any marker whose
bench is the `highlightedBench` has the custom styling. (You can use `setLabel`
and `setIcon`.)

Pass `highlightedBench` to the `BenchList` as well. Add custom styling to
whichever `BenchListItem` corresponds to the `highlightedBench`.

Finally, pass `setHighlightedBench` to `BenchList`. On hovering over a
`BenchListItem`, set `highlightedBench` to that bench.

Congratulations! You finished! Give yourself a huge pat on the back and
celebrate by **committing your code!**
