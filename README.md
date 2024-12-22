# Elixir Enum.each and throw unexpected behavior

This example demonstrates a potential issue in Elixir when using `Enum.each` along with `throw`. The `throw` statement, intended to interrupt the loop when a condition is met, doesn't always behave as expected.  The `IO.puts` statement after the conditional is still executed even after the `throw` is called.

## Solution

The solution demonstrates using `Enum.reduce` for proper iteration control, halting when an error condition is met.