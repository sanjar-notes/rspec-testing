---
id: vNui4B6mu9fSjYI4Y5pBS
title: Matchers
desc: ''
updated: 1643270133537
created: 1643268996710
---

## What's a matcher
- Matchers are nothing but a DSL for specifying expectations of tests.
- They all evaulate properly or mess up, causing errors.

There are two sides to a matcher:
1. Actual value
2. Expected value

There are many kinds of matchers, because there are many kinds of objects and operations.

1. Equality
```ruby
# Note: there's no == 🙃
expect(actual).to eq(expected) # .eq

expect(actual).to equal(expected) #.equal
expect(actual).to be(expected) # same as above

expect(actual).to
```
2. Truthiness and bool values
```ruby
expect(actual).to be_truthy
# not nil or false - the two falsey values in ruby

expect(actual).to be_falsey
# nil or false

expect(actual).to be true # strictly boolean true
expect(actual).to be false # strictly boolean false
```
3. Comparisons
```ruby
# eq(already done)
expect(actual).to be > expected
expect(actual).to be < expected
expect(actual).to be >= expected
expect(actual).to be <= expected

# in range check
expect(actual).to be_between(min, max).inclusive
expect(actual).to be_between(min, max).exclusive

# neighbourhood delta
expect(actual).to be_within(delta).of(expected)

# regex match
expect(actual).to match(/regexp/)
```
4. Existentialism
```ruby
expect(actual).to be_nil

expect
```
5. Objects
```ruby

```
