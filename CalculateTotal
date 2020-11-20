import tkinter
import tkinter.messagebox

def main():
    automotive_options()
class automotive_options:
    def __init__(self):
        self.main_window = tkinter.Tk() # create main window

        self.top_frame = tkinter.Frame(self.main_window) # create top frame
        self.bottom_frame = tkinter.Frame(self.main_window) # create main window

        # create checkbox objects
        self.checkbox1_var = tkinter.IntVar()
        self.checkbox2_var = tkinter.IntVar()
        self.checkbox3_var = tkinter.IntVar()
        self.checkbox4_var = tkinter.IntVar()
        self.checkbox5_var = tkinter.IntVar()
        self.checkbox6_var = tkinter.IntVar()
        self.checkbox7_var = tkinter.IntVar()

        # set checkbox objects to 0
        self.checkbox1_var.set(0)
        self.checkbox2_var.set(0)
        self.checkbox3_var.set(0)
        self.checkbox4_var.set(0)
        self.checkbox5_var.set(0)
        self.checkbox6_var.set(0)
        self.checkbox7_var.set(0)

        # create checkbox buttons and labels
        self.checkbox1 = tkinter.Checkbutton(self.top_frame, text="Oil Change - $30", variable=self.checkbox1_var, command=self.oil_change)
        self.checkbox2 = tkinter.Checkbutton(self.top_frame, text="Lube Job - $20", variable=self.checkbox2_var, command=self.lube_job)
        self.checkbox3 = tkinter.Checkbutton(self.top_frame, text="Radiator Flush - $40", variable=self.checkbox3_var, command=self.radiator_flush)
        self.checkbox4 = tkinter.Checkbutton(self.top_frame, text="Transmission Flush - $100", variable=self.checkbox4_var, command=self.transmission_flush)
        self.checkbox5 = tkinter.Checkbutton(self.top_frame, text="Inspection - $35", variable=self.checkbox5_var, command=self.inspection)
        self.checkbox6 = tkinter.Checkbutton(self.top_frame, text="Muffler Replacement - $200", variable=self.checkbox6_var, command=self.muffler_replacement)
        self.checkbox7 = tkinter.Checkbutton(self.top_frame, text="Tire Rotation - $20", variable=self.checkbox7_var, command=self.tire_rotation)

        # pack checkboxes
        self.checkbox1.pack()
        self.checkbox2.pack()
        self.checkbox3.pack()
        self.checkbox3.pack()
        self.checkbox4.pack()
        self.checkbox5.pack()
        self.checkbox6.pack()
        self.checkbox7.pack()

        # create and pack display charges and quit buttons
        self.display_charges_button = tkinter.Button(self.bottom_frame, text="Display Charges", command=self.display_charges) # TODO make function display_charges
        self.display_charges_button.pack(side="left")
        self.quit_button = tkinter.Button(self.bottom_frame, text="Quit", command=self.main_window.destroy)
        self.quit_button.pack(side="right")

        # create total IntVar and set total to 0.00
        self.total = tkinter.IntVar()
        self.total.set(0.00)

        # pack frames
        self.top_frame.pack()
        self.bottom_frame.pack()

        tkinter.mainloop()

    def display_charges(self): # function to display charges from checked boxes
        s = "Total Charges: $" + str(self.total.get())
        tkinter.messagebox.showinfo("Total Charges", s) # display messagebox of total charges

    # functions for each service and calculating total cost of selected services and setting total
    def oil_change(self):
        total = float(self.total.get())
        if self.checkbox1_var.get():
            total += 30
        total = format(total, ".2f")
        self.total.set(total)
    def lube_job(self):
        total = float(self.total.get())
        if self.checkbox2_var.get():
            total += 20
        total = format(total, ".2f")
        self.total.set(total)
    def radiator_flush(self):
        total = float(self.total.get())
        if self.checkbox3_var.get():
            total += 40
        total = format(total, ".2f")
        self.total.set(total)
    def transmission_flush(self):
        total = float(self.total.get())
        if self.checkbox4_var.get():
            total += 100
        total = format(total, ".2f")
        self.total.set(total)
    def inspection(self):
        total = float(self.total.get())
        if self.checkbox5_var.get():
            total += 35
        total = format(total, ".2f")
        self.total.set(total)
    def muffler_replacement(self):
        total = float(self.total.get())
        if self.checkbox6_var.get():
            total += 200
        total = format(total, ".2f")
        self.total.set(total)
    def tire_rotation(self):
        total = float(self.total.get())
        if self.checkbox7_var.get():
            total += 20
        total = format(total, ".2f")
        self.total.set(total)
main()
