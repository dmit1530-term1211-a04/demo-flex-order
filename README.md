# [demo] Flex Order

Understanding and using the flex order property with advanced CSS selectors

Things to note when going to use flex order:
- flex order is a property that gets applied to the flex-items (children).
- By default all flex-items start at zero (0).
- To use flex order and change up the order of the elements you must start with a negative integer (ie. -1)

For example, if you have 4 sections and you want to move them around, you could use flex order. Let's say for example by default the order of the sections are 1,2,3,4 but they need to be placed in this order: 3,4,2,1

You would start by doing this: 

``` css
/** you are taking the third section and placing it in the first position **/
section:nth-child(3) {
  order: -1;
}

/** then you keep following the of -1, 0, 1, 2.... **/

```

