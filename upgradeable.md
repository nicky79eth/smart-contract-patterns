# Upgradeable Contract Pattern

Upgradeable contracts allow developers to update logic after deployment.

This is important because smart contracts are immutable by default.

## Common Approach

Proxy Pattern:

- Proxy contract stores state
- Logic contract contains implementation
- Proxy delegates calls to logic contract

## Benefits

- fix bugs
- add new features
- improve protocol over time

## Risks

- upgrade authority abuse
- storage collision
- complexity
