import random

class Ball:
    def __init__(self, x, y):
        self.x = x
        self.y = y

    def move(self):
        self.x += random.uniform(-1, 1)
        self.y += random.uniform(-1, 1)

# Erstellen eines Balls mit Startposition (0, 0)
ball = Ball(0, 0)

# Simulationsschleife für 10 Schritte
for _ in range(10):
    ball.move()
    print(f"Position: ({ball.x}, {ball.y})")
