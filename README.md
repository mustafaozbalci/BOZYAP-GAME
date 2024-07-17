# BOZYAP-GAME
This project is a puzzle game that allows users to select an image file, divide it into multiple pieces, and then play a puzzle game to reassemble the image. The game uses tkinter for the user interface, PIL and pillow_heif for image processing, and pygame for the puzzle gameplay.

# Requirements
Python 3.x
Libraries: tkinter, PIL, pillow_heif, pygame, random, tempfile
Main Functions
split_image(image_path, piece_count):
This function splits a given image file into a specified number of pieces. It supports .heic or .heif formats using the pillow_heif module and other formats using the PIL module. The image is divided into equal-sized pieces and stored in a temporary folder.

# Parameters:
image_path (str): Path to the image file.
piece_count (int): Number of pieces for the puzzle.
Returns:
piece_paths (list): List of paths to the piece files.
cols (int): Number of columns.
rows (int): Number of rows.
run_puzzle(piece_paths, cols, rows): 
This function runs the puzzle game using pygame. It randomly arranges the pieces and lets the user reassemble them correctly.

# Parameters:
piece_paths (list): List of paths to the piece files.
cols (int): Number of columns.
rows (int): Number of rows.
main(): 
This function creates the user interface using tkinter. It allows the user to select an image file and specify the number of pieces. Then it starts the puzzle game.

# Features:
File dialog to select the image file.
Entry field to specify the number of pieces.
Button to start the puzzle game.

# User Interface Components
info_label: Label to inform the user to select an image file.
select_image_button: Button to open the file dialog to select an image.
image_path_label: Label to display the path of the selected image file.
piece_count_info_label: Label to inform the user to enter the number of pieces.
piece_count_entry: Entry field to input the number of pieces.
start_puzzle_button: Button to start the puzzle game.
