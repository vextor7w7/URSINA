<h1 align="center"> the rats of the games</h1>
<h3 align="izquierda">DESCRIPCION</h3>
Este es un grupo que intenta copiar todo juego existente 
a base de ursina en este caso comenzamos por minecraft.

<h3 align="izquierda">PARTICIPANTES</h3>
- Diego Paz
- Victor Casas

<h3 align="izquierda">Instrucciones para ejecutar el proyecto</h3>
el proyecto puede correr con cualquier version de python que acepte ursina
- dar f5 para comenzar
- click derecho romper
- click izquierdo pones ladrillos


<h3 align="izquierda">CODIGO</h3>
from ursina import *
from ursina.prefabs.first_person_controller \
  import FirstPersonController

app = Ursina()
Sky()
player = FirstPersonController()
window.fullscreen = True
arm = Entity(
  parent=camera.ui,
  model='cube',
  color=color.yellow,
  position=(0.75, -0.6),
  rotation= (150, -10,6),
  scale = (0.2,0.2,1.5)
)
def update():
  if held_keys['left mouse']:
    arm.position = (0.6, -0.5)
  elif held_keys['right mouse']:
    arm.position = (0.6, -0.5)
  else:
    arm.position = (0.75, -0.6)

boxes = []
###########
lado = 25
###########
for n in range(lado):
  for k in range(lado):
    box = Button(
      position=(k, 0, n),
      color=color.green,
      highlight_color=color.lime,
      model='cube',
      texture=
      load_texture('grass'),
      origin_y=0.5,
      parent=scene
    )
    boxes.append(box)

def input(key):
  for box in boxes:
    if box.hovered:
      if key == 'left mouse down':
        newBox = Button(
          position=
          box.position + mouse.normal,
          color=color.orange,
          highlight_color=color.lime,
          model='cube',
          texture=
          load_texture('brick'),
          origin_y=0.5,
          parent=scene
        )
        boxes.append(newBox)
      if key == 'right mouse down':
        boxes.remove(box)
        destroy(box)
Tree=Entity(color=color.brown,highlight_color=color.lime,model='cube',position=(0+lado/2, 0, 0+lado/2),texture= 'white_cube',parent=scene)
Tree=Entity(color=color.brown, highlight_color=color.lime,model='cube',position=(0+lado/2, 1, 0+lado/2),texture= 'white_cube',parent=scene)
Tree=Entity(color=color.brown, highlight_color=color.lime,model='cube',position=(0+lado/2, 2, 0+lado/2),texture= 'white_cube',parent=scene)        
Tree=Entity(color=color.brown, highlight_color=color.lime,model='cube',position=(0+lado/2, 3, 0+lado/2),texture= 'white_cube',parent=scene)        
Tree=Entity(color=color.brown, highlight_color=color.lime,model='cube',position=(0+lado/2, 4, 0+lado/2),texture= 'white_cube',parent=scene)
Tree=Entity(color=color.brown, highlight_color=color.lime,model='cube',position=(0+lado/2, 5, 0+lado/2),texture= 'white_cube',parent=scene)
Tree=Entity(color=color.green, highlight_color=color.lime,model='cube',position=(1+lado/2, 4, 0+lado/2),texture= 'white_cube',parent=scene)
Tree=Entity(color=color.green, highlight_color=color.lime,model='cube',position=(-1+lado/2, 4, 0+lado/2),texture= 'white_cube',parent=scene)
Tree=Entity(color=color.green, highlight_color=color.lime,model='cube',position=(2+lado/2, 4, 0+lado/2),texture= 'white_cube',parent=scene)
Tree=Entity(color=color.green, highlight_color=color.lime,model='cube',position=(-2+lado/2, 4, 0+lado/2),texture= 'white_cube',parent=scene)
Tree=Entity(color=color.green, highlight_color=color.lime,model='cube',position=(1+lado/2, 5, 0+lado/2),texture= 'white_cube',parent=scene)
Tree=Entity(color=color.green, highlight_color=color.lime,model='cube',position=(-1+lado/2, 5, 0+lado/2),texture= 'white_cube',parent=scene)
Tree=Entity(color=color.green, highlight_color=color.lime,model='cube',position=(1+lado/2, 6, 0+lado/2),texture= 'white_cube',parent=scene)
Tree=Entity(color=color.green, highlight_color=color.lime,model='cube',position=(0+lado/2, 6, 0+lado/2),texture= 'white_cube',parent=scene)
Tree=Entity(color=color.green, highlight_color=color.lime,model='cube',position=(-1+lado/2, 6, 0+lado/2),texture= 'white_cube',parent=scene)
Tree=Entity(color=color.green, highlight_color=color.lime,model='cube',position=(0+lado/2, 4, 1+lado/2),texture= 'white_cube',parent=scene)
Tree=Entity(color=color.green, highlight_color=color.lime,model='cube',position=(0+lado/2, 4, -1+lado/2),texture= 'white_cube',parent=scene)
Tree=Entity(color=color.green, highlight_color=color.lime,model='cube',position=(0+lado/2, 5, 1+lado/2),texture= 'white_cube',parent=scene)
Tree=Entity(color=color.green, highlight_color=color.lime,model='cube',position=(0+lado/2, 5, -1+lado/2),texture= 'white_cube',parent=scene)
Tree=Entity(color=color.green, highlight_color=color.lime,model='cube',position=(0+lado/2, 6, 2+lado/2),texture= 'white_cube',parent=scene)
Tree=Entity(color=color.green, highlight_color=color.lime,model='cube',position=(0+lado/2, 6, -2+lado/2),texture= 'white_cube',parent=scene)
Tree=Entity(color=color.green, highlight_color=color.lime,model='cube',position=(3+lado/2, 4, 0+lado/2),texture= 'white_cube',parent=scene)
Tree=Entity(color=color.green, highlight_color=color.lime,model='cube',position=(-3+lado/2, 4, 0+lado/2),texture= 'white_cube',parent=scene)
Tree=Entity(color=color.green, highlight_color=color.lime,model='cube',position=(4+lado/2, 4, 0+lado/2),texture= 'white_cube',parent=scene)
Tree=Entity(color=color.green, highlight_color=color.lime,model='cube',position=(-4+lado/2, 4, 0+lado/2),texture= 'white_cube',parent=scene)
Tree=Entity(color=color.green, highlight_color=color.lime,model='cube',position=(-2+lado/2, 5, 0+lado/2),texture= 'white_cube',parent=scene)
Tree=Entity(color=color.green, highlight_color=color.lime,model='cube',position=(2+lado/2, 5, 0+lado/2),texture= 'white_cube',parent=scene)
Tree=Entity(color=color.green, highlight_color=color.lime,model='cube',position=(0+lado/2, 4, 3+lado/2),texture= 'white_cube',parent=scene)
Tree=Entity(color=color.green, highlight_color=color.lime,model='cube',position=(0+lado/2, 4, -3+lado/2),texture= 'white_cube',parent=scene)
Tree=Entity(color=color.green, highlight_color=color.lime,model='cube',position=(0+lado/2, 5, 3+lado/2),texture= 'white_cube',parent=scene)
Tree=Entity(color=color.green, highlight_color=color.lime,model='cube',position=(0+lado/2, 5, -3+lado/2),texture= 'white_cube',parent=scene)
Tree=Entity(color=color.green, highlight_color=color.lime,model='cube',position=(4+lado/2, 4, 0+lado/2),texture= 'white_cube',parent=scene)
app.run()
