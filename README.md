import tkinter as tk

root = tk.Tk()
root.title("Simple Tkinter Program")
root.geometry("300x200")  # Width x Height
root.resizable(False,False)

def on_button_click():
    user_input = entry.get()  
    label_output.config(text=f"Hello, {user_input}!") 


label = tk.Label(root, text="Enter your name:", font=("Arial", 12))
label.pack()


entry = tk.Entry(root, font=("Arial", 12))
entry.pack(pady=5)


button = tk.Button(root, text="Me", command=on_button_click, font=("Arial", 12))
button.pack(pady=10)


label_output = tk.Label(root, text="", font=("Arial", 12), fg="green")
label_output.pack(pady=10)


root.mainloop()