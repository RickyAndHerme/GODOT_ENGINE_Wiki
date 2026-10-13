# ブロック崩しゲームの制作

Godot 4.xを使ってブロック崩しを制作する。

## 1. シーン構成

以下のノードを使用する。

- Node2D
- CharacterBody2D
- CollisionShape2D

## 2. プレイヤーの移動

```gdscript
func _physics_process(delta):
    var direction = Input.get_axis("ui_left", "ui_right")
    velocity.x = direction * 300
    move_and_slide()
```

## 3. 画像の挿入

![シーン構成](images/blockbreak.png)
