# Reusable 3D Models for Blender

## Objective

Build reusable 3D models that can be edited later in Blender and exported to any game engine.

The models must remain fully editable after the script is executed.

The user must be able to open the `.blend` file and manually modify any object.

## Workflow

Always follow this workflow:

1. Generate a complete Python script.
2. Clear the scene before creating objects.
3. Create all objects through the Blender API.
4. Organize the scene.
5. Create materials.
6. Organize collections.
7. Correctly position origins and pivots.
8. Apply scale and rotation when necessary.
9. Save the `.blend` file when requested.
10. Export to `.fbx`, `.glb`, `.obj`, or other formats when requested.

## Code

All code must be:

- Organized
- Commented
- Divided into functions
- Reusable
- Easy to modify
- Compatible with recent Blender versions

Avoid code repetition.

Always reuse functions.

Always use descriptive names.

Never leave objects named `Cube`, `Cube.001`, `Material.001`, and so on.

## Modeling

Always prefer procedural modeling.

Use simple primitives whenever possible.

Examples:

- Cube
- Cylinder
- Cone
- Plane
- UV Sphere
- Ico Sphere

Avoid extremely dense geometry when it is not necessary.

When possible, expose parameters at the beginning of the script to make future modifications easier.

Examples:

- Height
- Width
- Thickness
- Segment count
- Detail count

## Organization

Always:

- Name objects
- Name materials
- Name collections
- Keep the hierarchy clean

Never produce disorganized scenes.

## Philosophy

Prioritize:

- Reuse
- Clarity
- Simplicity
- Ease of maintenance

The script must be treated as production code.
