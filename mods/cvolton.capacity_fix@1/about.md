# CapacityFix

* Fixes an issue with an optimization that RobTop messed up during the development.
* This only fixes the behavior when High Capacity Mode is DISABLED.
* It might help with RAM usage or stutters, the real world effect of this optimization hasn't been measured yet.
* Credits to Wyliemaster for noticing the issue in the first place.

## Documentation
This patches GJBaseGameLayer::updateLayerCapacity to fix an issue where RobTop misaligned most items loaded in this function by 1 from how they are saved when saving the extraString field for the level.

Since the issue is as simple as this, using a series of binary patches has been deemed simpler and easier to manage than rewriting the whole function from scratch.

What this function does is that it splits the extraString field and assigns elements from there as class members into GJBaseGameLayer.