## 0.3.0
- `ir::Component` takes a `has_interface` argument and ensures that interface ports are present when it is true.
- The `Visitor` trait supports new `start_context` and `finish_context` methods which allow the pass to affect the context before and after the components are visited respectively.
- New `wrap-main` pass that generates a top-level `main` component if the top-level component is not named that.
- Pretty printer prints code more tersely.

## 0.2.1
- Remove necessary indentation inlined verilog primitives
- Add new `discover-external` pass to transform inlined cells into `@external` cells
- Implementation of `static` primitives and components and finish work on static milestone paving way for deprecation of the `@static` attribute.

## 0.2.0
- The core compilation primitives are included in the compiler distribution eliminating reliance on the primitives path.
- Add new `data-path-infer` pass to infer `@data` annotation allowing more backend optimization
- Distribute `calyx` and `futil` binaries together and show deprecation warning for the latter.

## 0.1.0
- Initial release with seperate Calyx crates and the new `static` primitives