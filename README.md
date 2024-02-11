import pygame

# Define some colors
BLACK = (0, 0, 0)
WHITE = (255, 255, 255)

# Initialize the pygame library
pygame.init()

# Create a display surface
screen = pygame.display.set_mode((640, 480))

# Set the background color
screen.fill(WHITE)

# Create a circle object
circle = pygame.draw.circle(screen, BLACK, (320, 240), 100)

# Loop until the user quits
while True:
    # Check for events
    for event in pygame.event.get():
        # If the user quits, quit the game
        if event.type == pygame.QUIT:
            pygame.quit()
            exit()

    # Update the screen
    pygame.display.update()
    
