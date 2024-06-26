# `CheatSpan`

```rust
enum CheatSpan {
    Indefinite: (),
    TargetCalls: usize
}
```

`CheatSpan` is an enum used to specify for how long the target should be cheated for.
- `Indefinite` applies the cheatcode indefinitely, until the cheat is canceled manually (e.g. using `stop_warp`).
- `TargetCalls` applies the cheatcode for a specified number of calls to the target, after which the cheat is canceled (or until the cheat is canceled manually).

> 📝 **Note**
> 
> `CheatTarget::All` can only be used with `CheatSpan::Indefinite`.
>
