# MicroDuck assets

来源：[pollen-robotics/microduck_rl](https://github.com/pollen-robotics/microduck_rl)
路径：`src/mjlab_microduck/robot/microduck/`（`robot_walk.xml` + `assets/`）

- `MicroDuck.xml`：由 `robot_walk.xml` 改 `meshdir=meshes`
- `scene.xml`：由 `scene_walk.xml` 改 include
- `urdf/MicroDuck.urdf`：用 **mjcf-to-urdf** 从 MJCF 转换（折叠 mesh 居中偏移；见 `scripts/mjcf_to_urdf_microduck.py`）

重转 URDF：

```bash
.venv_tools/bin/python scripts/mjcf_to_urdf_microduck.py
```
