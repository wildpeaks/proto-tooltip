# Tooltip

VRML PROTO (based on `IndexedFaceSet`) that **generates a rounded rectangle with a tip** that visually links to an arbitrary 3D position.

The side where the tip is attached to the rectangle is **automatically deduced from the relative position** of the target.

	EXTERNPROTO Tooltip [
		exposedField  SFVec3f  center
		exposedField  SFVec3f  tip
		exposedField  SFVec2f  size
		exposedField  SFFloat  radius
		field         SFBool   solid
	] "proto.Tooltip.wrl#Tooltip"


-------------------------------------------------------------------------------

## Property `center`

**3D position of the center** of the rounded rectangle.

Definition:
 - Field Type: `exposedField`
 - Data Type: `SFVec3f`
 - Default Value: `0 0 0`


-------------------------------------------------------------------------------

## Property `tip`

**3D position of the tip** of the triangle attached outside the rounded rectangle.

Definition:
 - Field Type: `exposedField`
 - Data Type: `SFVec3f`
 - Default Value: `0 0 0`


-------------------------------------------------------------------------------

## Property `size`

**Width & height** of the inner area of the rounded rectangle.

You could use [MonospaceText.bboxSize](https://github.com/wildpeaks/proto-monospacetext#event-bboxsize)
to fit a tooltip around an arbitrary text.

Definition:
 - Field Type: `exposedField`
 - Data Type: `SFVec3f`
 - Default Value: `2 2`


-------------------------------------------------------------------------------

## Property `radius`

**Radius** of the rounded border of the rectangle.

Definition:
 - Field Type: `exposedField`
 - Data Type: `SFVec3f`
 - Default Value: `1`


-------------------------------------------------------------------------------

## Property `solid`

Like `IndexedFaceSet.solid`, renders both sides (`FALSE`) or only the front side (`TRUE`).

Definition:
 - Field Type: `field`
 - Data Type: `SFBool`
 - Default Value: `TRUE`


-------------------------------------------------------------------------------

