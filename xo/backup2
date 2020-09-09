import pygame

def checkmouseclick():
    for event in pygame.event.get():
        if event.type == pygame.MOUSEBUTTONDOWN:
            return True

def drawx(p1):
    if p1 == 1:
        pygame.draw.line(screen, white, (150, 150), (344, 344), 5)
        pygame.draw.line(screen, white, (344, 150), (150, 344), 5)
    if p1 == 2:
        pygame.draw.line(screen, white, (353, 150), (547, 344), 5)
        pygame.draw.line(screen, white, (547, 150), (353, 344), 5)
    if p1 == 3:
        pygame.draw.line(screen, white, (556, 150), (750, 344), 5)
        pygame.draw.line(screen, white, (750, 150), (556, 344), 5)
    if p1 == 4:
        pygame.draw.line(screen, white, (150, 353), (344, 547), 5)
        pygame.draw.line(screen, white, (344, 353), (150, 547), 5)
    if p1 == 5:
        pygame.draw.line(screen, white, (353, 353), (547, 547), 5)
        pygame.draw.line(screen, white, (547, 353), (353, 547), 5)
    if p1 == 6:
        pygame.draw.line(screen, white, (556, 353), (750, 547), 5)
        pygame.draw.line(screen, white, (750, 353), (556, 547), 5)
    if p1 == 7:
        pygame.draw.line(screen, white, (150, 556), (344, 750), 5)
        pygame.draw.line(screen, white, (344, 556), (150, 750), 5)
    if p1 == 8:
        pygame.draw.line(screen, white, (353, 556), (547, 750), 5)
        pygame.draw.line(screen, white, (547, 556), (353, 750), 5)
    if p1 == 9:
        pygame.draw.line(screen, white, (556, 556), (750, 750), 5)
        pygame.draw.line(screen, white, (750, 556), (556, 750), 5)

def drawo(p2):
    if p2 == 1:
        pygame.draw.circle(screen, white, (247, 247), 92, 5)
    if p2 == 2:
        pygame.draw.circle(screen, white, (450, 247), 92, 5)
    if p2 == 3:
        pygame.draw.circle(screen, white, (653, 247), 92, 5)
    if p2 == 4:
        pygame.draw.circle(screen, white, (247, 450), 92, 5)
    if p2 == 5:
        pygame.draw.circle(screen, white, (450, 450), 92, 5)
    if p2 == 6:
        pygame.draw.circle(screen, white, (653, 450), 92, 5)
    if p2 == 7:
        pygame.draw.circle(screen, white, (247, 653), 92, 5)
    if p2 == 8:
        pygame.draw.circle(screen, white, (450, 653), 92, 5)
    if p2 == 9:
        pygame.draw.circle(screen, white, (653, 653), 92, 5)

def table():
    pygame.draw.line(screen, (255, 255, 255), (150, 344), (750, 344), 9)
    pygame.draw.line(screen, (255, 255, 255), (150, 547), (750, 547), 9)
    pygame.draw.line(screen, (255, 255, 255), (344, 150), (344, 750), 9)
    pygame.draw.line(screen, (255, 255, 255), (547, 150), (547, 750), 9)

def choose(mousex,mousey):
    if mousex <=344 and mousex>=150 and mousey<=344 and mousey>=150:
        x = 1
    elif mousex <=547 and mousex>=353 and mousey<=344 and mousey>=150:
        x = 2
    elif mousex <=750 and mousex>=556 and mousey<=344 and mousey>=150:
        x = 3
    elif mousex <=344 and mousex>=150 and mousey<=547 and mousey>=353:
        x = 4
    elif mousex <=547 and mousex>=353 and mousey<=547 and mousey>=353:
        x = 5
    elif mousex <=750 and mousex>=556 and mousey<=547 and mousey>=353:
        x = 6
    elif mousex <=344 and mousex>=150 and mousey<=750 and mousey>=556:
        x = 7
    elif mousex <=547 and mousex>=353 and mousey<=750 and mousey>=556:
        x = 8
    elif mousex <=750 and mousex>=556 and mousey<=750 and mousey>=556:
        x = 9
    else:
        x = False

    return x

def choosex(p1):
    for n, i in enumerate(tableraw):
        if p1 == n+1:
            if i == "o" or i == "x":
                return False
                #adica nu e bine
            else:
                tableraw[n] = "x"
    return True

def chooseo(p2):
    for n, i in enumerate(tableraw):
        if p2 == n+1:
            if i == "x" or i == "o":
                return False
            else:
                tableraw[n] = "o"
    return True

def wincheckx():
    if tableraw[0] == "x" and tableraw[1] == "x" and tableraw[2]=="x":
        return True
    if tableraw[3] == "x" and tableraw[4] == "x" and tableraw[5]=="x":
        return True
    if tableraw[6] == "x" and tableraw[7] == "x" and tableraw[8]=="x":
        return True
    if tableraw[0] == "x" and tableraw[3] == "x" and tableraw[6]=="x":
        return True
    if tableraw[1] == "x" and tableraw[4] == "x" and tableraw[7]=="x":
        return True
    if tableraw[2] == "x" and tableraw[5] == "x" and tableraw[8]=="x":
        return True
    if tableraw[0] == "x" and tableraw[4] == "x" and tableraw[8]=="x":
        return True
    if tableraw[2] == "x" and tableraw[4] == "x" and tableraw[6]=="x":
        return True
    return False

def winchecko():
    if tableraw[0] == "o" and tableraw[1] == "o" and tableraw[2]=="o":
        return True
    if tableraw[3] == "o" and tableraw[4] == "o" and tableraw[5]=="o":
        return True
    if tableraw[6] == "o" and tableraw[7] == "o" and tableraw[8]=="o":
        return True
    if tableraw[0] == "o" and tableraw[3] == "o" and tableraw[6]=="o":
        return True
    if tableraw[1] == "o" and tableraw[4] == "o" and tableraw[7]=="o":
        return True
    if tableraw[2] == "o" and tableraw[5] == "o" and tableraw[8]=="o":
        return True
    if tableraw[0] == "o" and tableraw[4] == "o" and tableraw[8]=="o":
        return True
    if tableraw[2] == "o" and tableraw[4] == "o" and tableraw[6]=="o":
        return True
    return False

def tiecheck():
    if tableraw[0] != "-" and tableraw[1] != "-" and tableraw[2] != "-" and tableraw[3] != "-" and tableraw[4] != "-" and tableraw[5] != "-" and tableraw[6] != "-" and tableraw[7] != "-" and tableraw[8] != "-":
        return True
    return False

pygame.init()
screen = pygame.display.set_mode((900,900))
screen.fill((0, 0, 0))
pygame.display.set_caption("Tic Tac Toe")
pygame.display.set_icon(pygame.image.load('icon.png'))
white = (255,255,255)
tableraw = ["-", "-", "-", "-", "-", "-", "-", "-", "-"]
myfont = pygame.font.SysFont('Comic Sans', 30, False)


#THIS IS WHERE THE GAME BEGINS!!
running = True
while running:
    table()
    pygame.display.update()
    playerone = True
    playertwo = True
#PLAYER_ONE
    while playerone:
        if checkmouseclick():
            p1mousex, p1mousey = pygame.mouse.get_pos()
            p1 = choose(p1mousex, p1mousey)
            print("MOUSE1 = ", p1)
            if p1 == False:
                print("Out of bounds!")
            elif choosex(p1):
                drawx(p1)
                pygame.display.update()
                playerone = False
                textsurface = myfont.render('Choose another box!', False, (0, 0, 0))
                screen.blit(textsurface, (294, 15))
                pygame.display.update()
            else:
                print("Choose another box!")
                textsurface = myfont.render('Choose another box!', False, (255, 0, 255))
                screen.blit(textsurface, (294, 15))
                pygame.display.update()


    if wincheckx():
        print("Player one won!")
        textsurface = myfont.render('Player one won!', False, (0, 0, 255))
        screen.blit(textsurface, (294, 15))
        pygame.display.update()
        playertwo = False
        playerone = False

    if tiecheck() and wincheckx() == False:
        print("It's a tie")
        textsurface = myfont.render("It's a tie!", False, (0, 255, 0))
        screen.blit(textsurface, (343, 15))
        pygame.display.update()
        playertwo = False
        playerone = False

    pygame.display.update()
#PLAYER_TWO
    while playertwo:
        if checkmouseclick():
            p2mousex, p2mousey = pygame.mouse.get_pos()
            p2 = choose(p2mousex, p2mousey)
            print("MOUSE2 = ", p2)
            if p2 == False:
                print("Out of bounds!")
            elif chooseo(p2):
                drawo(p2)
                pygame.display.update()
                playertwo = False
                textsurface = myfont.render('Choose another box!', False, (0, 0, 0))
                screen.blit(textsurface, (294, 15))
                pygame.display.update()
            else:
                print("Choose another box!")
                textsurface = myfont.render('Choose another box!', False, (255, 0, 255))
                screen.blit(textsurface, (294, 15))
                pygame.display.update()
    if winchecko():
        print("Player two won!")
        textsurface = myfont.render('Player two won!', False, (255, 0, 0))
        screen.blit(textsurface, (294, 15))
        pygame.display.update()
        playerone = False
        playertwo = False
