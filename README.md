# Godot Easing Functions

This addon provides a collection of commonly used easing functions for Godot Engine, written in GDScript. These functions allow for smooth transitions and animations by adjusting the interpolation curve of values over time.

## 📦 Installation

1. Clone or download this repository into your Godot project's `addons/` folder:

   ```bash
   git clone https://github.com/nodlag/godot-easing-functions.git
   ```


## 📁 File Structure

```
/addons/easing_functions/easing_functions.gd
```

This script contains a static class with multiple easing functions.

## 🚀 Usage


### Example: Smooth Movement with Easing

```gdscript
extends Node2D

var t := 0.0

func _process(delta):
    t = clamp(t + delta * 0.5, 0, 1)
    var eased_t = EasingFunctions.ease_out_cubic(t)
    position.x = lerp(100, 400, eased_t)
```

This moves a node from x = 100 to x = 400 using a cubic easing curve.

## 📚 Available Functions

All functions take a float `t` in the range `[0.0, 1.0]` and return a float also between `[0.0, 1.0]`.

- `linear(t)`
- `ease_in_sine(t)`
- `ease_out_sine(t)`
- `ease_in_out_sine(t)`
- `ease_in_quad(t)`
- `ease_out_quad(t)`
- `ease_in_out_quad(t)`
- `ease_in_cubic(t)`
- `ease_out_cubic(t)`
- `ease_in_out_cubic(t)`
- `ease_in_quart(t)`
- `ease_out_quart(t)`
- `ease_in_out_quart(t)`
- `ease_in_quint(t)`
- `ease_out_quint(t)`
- `ease_in_out_quint(t)`
- `ease_in_expo(t)`
- `ease_out_expo(t)`
- `ease_in_out_expo(t)`
- `ease_in_circ(t)`
- `ease_out_circ(t)`
- `ease_in_out_circ(t)`
- `ease_in_back(t)`
- `ease_out_back(t)`
- `ease_in_out_back(t)`
- `ease_in_elastic(t)`
- `ease_out_elastic(t)`
- `ease_in_out_elastic(t)`
- `ease_in_bounce(t)`
- `ease_out_bounce(t)`
- `ease_in_out_bounce(t)`

## 📝 License

This project is licensed under the MIT License.  
See the [LICENSE](LICENSE) file for more information.

## 🤝 Contributions

Contributions are welcome!  
Feel free to open issues or submit pull requests to add new easing functions or improvements.
