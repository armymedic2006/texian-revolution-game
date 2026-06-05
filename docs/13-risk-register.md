# Risk Register

| Risk | Impact | Mitigation | Test Coverage |
|---|---|---|---|
| Simultaneous turn resolution becomes too complex | Broken or unfair outcomes | Implement deterministic resolver with clear priority stages | Turn-resolution integration tests |
| Hidden orders leak in hot-seat mode | Multiplayer unfairness | Lock-order and pass-device privacy screen | UI privacy-state tests |
| Fog of war creates edge cases | Units/actions revealed incorrectly | Central LOS visibility calculation | LOS/fog tests |
| AI cheats unintentionally | Player distrust | AI uses only visibility API | AI information-access tests |
| Modifier stacking creates extreme balance swings | Unstable gameplay | Accept uncapped stacking by design, expose values for tuning | Modifier calculation tests |
| Santa Anna special rules create instant-win bugs | Incorrect victory | Explicit Santa Anna outcome checks | Victory condition tests |
| Victory point timers reset incorrectly | Bad wins/losses | Dedicated VP state machine | Capture/contest/reset tests |
| Free movement/pathing is hard without grid | Units clip through objects | Use obstacle-aware pathfinding and collision tests | Movement/path tests |
| Artillery/structure interactions are complex | Map state bugs | Structure damage state machine | Artillery/structure tests |
| Browser performance degrades | Slow resolution | Keep core logic decoupled from rendering | Performance smoke tests |
| UI/animation TDD slows implementation | Development friction | Separate pure UI state tests from rendering tests where possible | Component/state tests |
| Historical accuracy conflicts with alternate-history balance | Design confusion | Label historical vs gameplay assumptions clearly | Documentation review checklist |
| Hot-seat hidden information is exposed during resolution | Unfair multiplayer | Show only neutral/revealed actions | Resolution visibility tests |
| Officer rules create too many special cases | Bugs and balance problems | Isolate officer rules in dedicated systems | Officer behavior tests |
| Cavalry inside Alamo creates pathing problems | Movement bugs | Restrict by obstacle clearance and terrain type | Cavalry pathing tests |
