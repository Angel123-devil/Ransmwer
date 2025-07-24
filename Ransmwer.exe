# Ransmwer
test on the virtual machine on ransmower on pth
import tkinter as tk
from tkinter import messagebox
import time

# Funkce pro falešnou kontrolu hesla
def check_code():
    code = entry.get()
    if code == "kx666":
        messagebox.showinfo("Success", "Access Granted")
    elif code.lower() == "pay me":
        messagebox.showinfo("Payment", "Payment fake accepted.")
    else:
        messagebox.showerror("Error", "Wrong code. Try again.")

# První okno: fullscreen Windows 10 loading (falešné)
def show_loading_screen():
    loading = tk.Tk()
    loading.attributes('-fullscreen', True)
    loading.configure(bg="black")

    tk.Label(loading, text="Restarting Windows 10...", font=("Segoe UI", 30), fg="white", bg="black").pack(expand=True)

    loading.after(3000, lambda: [loading.destroy(), show_ransomware_screen()])
    loading.mainloop()

# Druhé okno: ransomware varování
def show_ransomware_screen():
    root = tk.Tk()
    root.attributes('-fullscreen', True)
    root.configure(bg="black")

    # Emoji rakve a oheň
    coffin_label = tk.Label(root, text="💀🔥", font=("Arial", 100), bg="black", fg="red")
    coffin_label.pack(pady=20)

    # Hlavní text
    warning = "IF YOU WANT IT NOT TO BE HERE,\nTURN IT ON FOR 20 BTC\n\nOTHERWISE WE WILL DESTROY YOU\n\nHOW TO PAY US:\n1. GO TO THE DARK WEB\n2. OFFICIAL BTC20\n3. PUT IT IN THE BAR AND GIVE THE DECRYPT\n4. GIVE THE PASSWORD: kx666\n5. AND SEND IT"
    tk.Label(root, text=warning, font=("Courier", 18, "bold"), fg="white", bg="black", justify="center").pack(pady=20)

    # Vstup pro falešný kód
    global entry
    entry = tk.Entry(root, font=("Courier", 16), width=30, justify='center')
    entry.pack(pady=10)

    # Tlačítko pro odeslání
    tk.Button(root, text="Submit / Pay Me", font=("Courier", 14), command=check_code, bg="red", fg="white").pack(pady=10)

    # Spodní lišta (vizuální falešný prvek)
    bottom_frame = tk.Frame(root, bg="#222")
    bottom_frame.pack(side="bottom", fill="x")

    tk.Label(bottom_frame, text="Type your code or payment command below", font=("Segoe UI", 12), bg="#222", fg="white").pack(pady=5)

    root.mainloop()

# Spuštění simulace
show_loading_screen()
