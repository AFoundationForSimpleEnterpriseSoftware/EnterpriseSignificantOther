EnterpriseSignificantOther
==========================

a simple way to create objects representing significant others

Architecture
============
The library revolves around the `EnterpriseSignificantOtherFactory`
which uses various `SignificantOtherProviders` to create the correct
significant other for a given `EnterprisePerson`. the ESOFactory can
use various mechanisms to reduce when candidates from the providers
are eligible. These filters must implement the `EnterpriseSignificantOtherFilter`
interface.

Planned filters include:
  - `SexualOrientationFilter`, driven by the `SexualOrientationRegistry`
  - `CostPerDateFilter`
  - `PromiscuityFilter`
  - likely many others
