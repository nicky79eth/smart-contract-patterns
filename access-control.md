# Access Control Pattern

Access control ensures that only authorized users can execute certain functions in a smart contract.

## Common Roles

- Owner
- Admin
- User

## Example

Only the owner can call sensitive functions:

function setValue(uint256 _value) public onlyOwner {
    value = _value;
}

## Best Practices

- Use role-based access control (RBAC)
- Avoid hardcoding addresses
- Use libraries like OpenZeppelin Ownable or AccessControl

## Risks

- improper role assignment
- centralization risk
