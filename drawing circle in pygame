import pygame
from pygame.locals import *
from OpenGL.GL import *
from OpenGL.GLU import *
import math
import matplotlib.pyplot as plt

def points():
    glPointSize(5)
    glBegin(GL_POINTS)
    glColor3f(0.7,0.4,2.3)

    def circle(xc, yc, r):
        t = 0
        while (t <= 3.14 / 4):
            x = xc + r * math.cos(t)
            y = yc + r * math.sin(t)
            x = int(x + 0.5)
            y = int(y + 0.5)
            glColor3f(0.7, 0.4, 2.3)
            glVertex2f(x, y)
            glVertex2f(-x, y)
            glVertex2f(x, -y)
            glVertex2f(-x, -y)
            glVertex2f(y, x)
            glVertex2f(-y, x)
            glVertex2f(y, -x)
            glVertex2f(-y, -x)
            t = t + 0.1

    circle(0, 0, 30)

    glVertex2f(1.1, 1.1)
    glVertex2f(1.20, 1.18)
    glVertex2f(1.30, 1.28)
    glVertex2f(1.45, 1.38)
    glVertex2f(1.55, 1.48)
    glVertex2f(1.65, 1.58)
    glVertex2f(1.75, 1.68)
    glVertex2f(1.8, 1.78)
    glVertex2f(1.90, 1.88)
    glVertex2f(2.0, 1.98)
    glVertex2f(2.08,2.08)
    glVertex2f(2.08, 2.2)
    glVertex2f(1.98, 2.25)
    glVertex2f(1.88, 2.35)
    glVertex2f(1.78, 2.45)
    glVertex2f(1.68, 2.55)
    glVertex2f(1.58, 2.65)
    glVertex2f(1.45, 2.75)
    glVertex2f(1.35, 2.85)
    glVertex2f(1.25, 2.95)
    glVertex2f(1.05, 3.05)
    glVertex2f(2.08, 2.08)
    glVertex2f(.9, 1.1)
    glVertex2f(.7, 1.3)
    glVertex2f(.5, 1.5)
    glVertex2f(.3, 1.7)
    glVertex2f(.1, 1.9)
    glVertex2f(.1, 2.1)
    glVertex2f(.3, 2.3)
    glVertex2f(.5, 2.5)
    glVertex2f(.7, 2.7)
    glVertex2f(.9, 2.9)

    glEnd()

def main():
    pygame.init()
    display=(800,600)
    pygame.display.set_mode(display, DOUBLEBUF | OPENGL)
    gluPerspective(100,(display[0]/display[1]),0.1, 50.0)
    glTranslate(0.0,0.0,-5)
    while True:
        for event in pygame.event.get():
            if event.type==pygame.QUIT:
                pygame.quit()
                quit()
        #glRotatef(1,3,1,1)
        #glClear(GL COLOR BUFFER BIT)
        #Cube()
        points()
        pygame.display.flip()
        pygame.time.wait(10)
main()
