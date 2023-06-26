from ast import main
import instaloader
import colorama
from colorama import Fore, Style
from tqdm import tqdm
import time
import os
from sys import stdout as terminal
from time import sleep
from itertools import cycle
from threading import Thread
def get_user_name():

    return os.getlogin()

done = False

def animate():
    for c in cycle([Fore.LIGHTYELLOW_EX +'|',Fore.LIGHTYELLOW_EX + '/',Fore.LIGHTYELLOW_EX + '-',Fore.LIGHTYELLOW_EX + '\\']):
        if done:
            break
        terminal.write(Fore.LIGHTGREEN_EX + '\rloading ' + c)
        terminal.flush()
        sleep(0.1)
    terminal.flush()

t = Thread(target=animate)
t.start()
sleep(3)
done = True

def download_posts(username):
    loader = instaloader.Instaloader()
    loader.download_profile(username, profile_pic=False, fast_update=False)

    for root, dirs, files in os.walk(username):
        for file in files:
            file_extension = os.path.splitext(file)[1]
            if file_extension.lower() in ['.txt', '.xz', '.mp4']:
                os.remove(os.path.join(root, file))


def download_allposts(username):
    loader = instaloader.Instaloader()
    save_directory = os.path.join(username)
    os.makedirs(save_directory, exist_ok=True) 
    loader.download_profile(username, profile_pic=False, fast_update=False)


    for root, dirs, files in os.walk(username):
        for file in files:
            file_extension = os.path.splitext(file)[1]
            if file_extension.lower() in ['.txt', '.xz']:
                os.remove(os.path.join(root, file))

def download_reels(username):
    loader = instaloader.Instaloader()
    os.path.join('reels')
    loader.download_profile(username, profile_pic=False, fast_update=False)


    for root, dirs, files in os.walk(username):
        for file in files:
            file_extension = os.path.splitext(file)[1]
            if file_extension.lower() in ['.txt', '.xz' , '.jpg', '.jpeg', '.png']:
                os.remove(os.path.join(root, file))
                
def download_photos(username):
    loader = instaloader.Instaloader()
    os.path.join('reels')
    loader.download_profile(username, profile_pic=False, fast_update=False)

    for root, dirs, files in os.walk(username):
        for file in files:
            file_extension = os.path.splitext(file)[1]
            if file_extension.lower() in ['.txt', '.xz' , '.mp4']:
                os.remove(os.path.join(root, file))


def exit_program(signum, frame):
    print("Exiting the program...")
    time.sleep(4)  
    os._exit(0)



print(Fore.LIGHTYELLOW_EX + """
V1""", Fore.LIGHTMAGENTA_EX + """ 
   __  .__   __.      _______..___________.     ___                ______   .__   __.   ______  _______ 
  |  | |  \ |  |     /       ||           |    /   \              /  __  \  |  \ |  |  /      ||   ____|
  |  | |   \|  |    |   (----``---|  |----`   /  ^  \     ______ |  |  |  | |   \|  | |  ,----'|  |__   
  |  | |  . `  |     \   \        |  |       /  /_\  \   |______||  |  |  | |  . `  | |  |     |   __|  
  |  | |  |\   | .----)   |       |  |      /  _____  \          |  `--'  | |  |\   | |  `----.|  |____ 
  |__| |__| \__| |_______/        |__|     /__/     \__\          \______/  |__| \__|  \______||_______|
""" , Fore.LIGHTYELLOW_EX + "                                                                                   by ABDALRAHMAN125141")

print(Fore.BLUE + "Welcame to Insta-once© Tool" , Fore.LIGHTYELLOW_EX +"V1")
print("                                                                                                        ")     
print(Fore.LIGHTYELLOW_EX + "------------------------------------------------------------")

while True:
    print("                                                                                                        ")
    print(Fore.RED + "[ 1 ]", Fore.YELLOW + "Download posts (only image)")
    print(Fore.RED + "[ 2 ]", Fore.YELLOW + "Download  all posts")
    print(Fore.RED + "[ 3 ]", Fore.YELLOW + "Download photos")
    print(Fore.RED + "[ 4 ]", Fore.YELLOW + "Download reels")
    print(Fore.RED + "[ 5 ]", Fore.YELLOW + "Contact US for a problem")
    print(Fore.RED + "[ 6 ]", Fore.YELLOW + "HELP")
    print(Fore.RED + "[ 0 ]", Fore.YELLOW + "EXIT")
    print(Fore.GREEN + "-----------------------------")
    print("                                                                                                        ")

    
    option = input(Fore.LIGHTYELLOW_EX + "Enter the option number:")
    print("                                                                ")
   
    if option == '1':
        print("                                                                                                        ")
       
        username = input(Fore.LIGHTGREEN_EX + "Enter the target Instagram username: ")
        print("                                                                                                        ")
        print(Fore.LIGHTYELLOW_EX + "----------------------------------")
        print(f"{Fore.LIGHTMAGENTA_EX}Target neutralized 😈 {Fore.LIGHTGREEN_EX}{username} 😈")
        print(Fore.LIGHTYELLOW_EX + "----------------------------------")
        print("                                                           ")
        print("Downloading posts...")
        download_posts(username)
    elif option == '2':
        print("                                                                                                        ")
       
        username = input(Fore.LIGHTGREEN_EX + "Enter the target Instagram username: ")
        print("                                                                                                        ")
        print(Fore.LIGHTYELLOW_EX + "----------------------------------")
        print(f"{Fore.LIGHTMAGENTA_EX}Target neutralized 😈 {Fore.LIGHTGREEN_EX}{username} 😈")
        print(Fore.LIGHTYELLOW_EX + "----------------------------------")
        print("                                                           ")
        print("Downloading all posts...")
        download_allposts(username)

    elif option == '3':
        print("                                                                                                        ")
        username = input(Fore.LIGHTGREEN_EX + "Enter the target Instagram username: ")
        print("                                                                                                        ")
        print(Fore.LIGHTYELLOW_EX + "----------------------------------")
        print(f"{Fore.LIGHTMAGENTA_EX}Target neutralized 😈 {Fore.LIGHTGREEN_EX}{username} 😈")
        print(Fore.LIGHTYELLOW_EX + "----------------------------------")
        print("                                                                                                        ")
        print("Downloading photos...")
        download_photos(username)

    elif option == '4':
        print("                                                                                                        ")
        username = input(Fore.LIGHTGREEN_EX + "Enter the target Instagram username: ")
        print("                                                                                                        ")
        print(Fore.LIGHTYELLOW_EX + "----------------------------------")
        print(f"{Fore.LIGHTMAGENTA_EX}Target neutralized 😈 {Fore.LIGHTGREEN_EX}{username} 😈")
        print(Fore.LIGHTYELLOW_EX + "----------------------------------")
        print("                                                                                                        ")
        print("Downloading reels...")
        download_reels(username)

    elif option == '5':
            print(Fore.MAGENTA + "-------------------------------------------------")
            print(Fore.CYAN + "Contact US for a problem at [a6291088@gmail.com]")
            print(Fore.MAGENTA + "-------------------------------------------------")

    elif option == '6':
            print(Fore.WHITE + "Hello, you are using the latest version of the" , Fore.YELLOW + "insta-once")
            print(Fore.GREEN + "------------------------------------------------------------------------------------")
            print(Fore.MAGENTA + "With insta-once you can Download :")
            print(Fore.YELLOW + "reels")
            print(Fore.GREEN + "posts")
            print(Fore.MAGENTA + "photos")
            print(Fore.LIGHTRED_EX + "from any Instagram account in once ")
            print(Fore.GREEN + "------------------------------------------------------------------------------------")
            print(Fore.LIGHTRED_EX + "you only have to choose what suits you from the options by writing")
            print(Fore.LIGHTRED_EX + "the number next to the option, then enter the file path or The folder")
            print(Fore.LIGHTRED_EX + "that you want to download")
            print(Fore.GREEN + "------------------------------------------------------------------------------------")
            print(Fore.YELLOW + "--Note:" ,Fore.CYAN + "When you finish uploading photos, reels, and posts, go to the folder in which the media ")
            print(Fore.CYAN + "was saved and rename it,because when you download new items for the same username, you may lose the old ones.")
            print(Fore.MAGENTA + "---------------------------------------------------------------------------------------------------------------")
            print(Fore.YELLOW + "--Note:" ,Fore.lightGREEN + "if you find a login error , try to restart your device.")
            print(Fore.CYAN + "was saved and rename it,because when you download new items for the same username, you may lose the old ones.")
            print(Fore.MAGENTA + "---------------------------------------------------------------------------------------------------------------")
            print(Fore.LIGHTYELLOW_EX + "⚠⚠ Warning:" ,Fore.LIGHTRED_EX + ": We are not responsible for any illegal or malicious use of the tool")
            print(Fore.CYAN + "Hack the word")
            print(Fore.LIGHTRED_EX + "Abdalrahman125141")      
       

    elif option == '0':
        print(Fore.LIGHTMAGENTA_EX + "-------------------------------------------------------------------")
        print(Fore.YELLOW + "Thank you for using the HIDEFILE Tool!")
        print(Fore.CYAN + "Created by ABDALRAHMAN125141")
        print(Fore.LIGHTMAGENTA_EX + "-------------------------------------------------------------------")
        print(Fore.YELLOW + "Have a great day!")
        print()
        break

    else:
        print(Fore.RED +"Invalid option selected.")
    
def get_save_directory():
    default_directory = os.path.join('C:/Users', get_user_name())
    folder_name = input(Fore.LIGHTGREEN_EX + "Enter the folder name to save the outputs (leave empty for default): ")
    if folder_name.strip() == "":
        return default_directory
    else:
        return os.path.join(default_directory, folder_name)    

if __name__ == "__main__":
    main()
   
