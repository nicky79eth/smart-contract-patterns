# Pausable Pattern

The pausable pattern allows a contract to be stopped in case of emergency.

This is often used to mitigate damage during attacks.

## Example

function pause() public onlyOwner {
    paused = true;
}

function unpause() public onlyOwner {
    paused = false;
}

modifier whenNotPaused() {
    require(!paused, "Paused");
    _;
}

## Use Cases

- security incidents
- contract upgrades
- emergency shutdown

## Risks

- centralization
- misuse by admin
