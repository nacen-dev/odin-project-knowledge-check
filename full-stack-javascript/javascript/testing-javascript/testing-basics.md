# Testing Basics

## Knowledge Check

### What are the benefits of TDD?

TDD gives a lot of benefits I'll list a few below.

- Saves time on the long run
- Reduces Bugs
- Makes your code easier to refactor
- Gives confidence to developers as it gives a safety net

### What are some common jest matchers?

#### Most Common matchers
- `toBe` uses Object.is to test exact equality
- `toEqual` recursively checks every field of an object or an array

#### Truthiness
- `toBeNull` matches only null
- `toBeUndefined` matches only undefined
- `toBeDefined` is the opposite of toBeUndefined
- `toBeTruthy` matches anything that an if statement treats as true
- `toBeFalsy` matches anything that an if statement treats as false

#### Numbers

`toBeGreaterThan`
`toBeGreaterThanOrEqual`
`toBeLessThan`
`toBeLessThanOrEqual`

but for floating points, use `toBeCloseTo` instead of `toEqual`

#### Strings

`toMatch` - check strings against regular expressions

#### Arrays

`toContain` - check if an array contains a particular value

#### Exceptions

`toThrow` - checks if a function throws an error