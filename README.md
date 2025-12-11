# Jackfruit_problem
mini project 

#Anirudh Para PES1UG25CS068

#Anurag Holla PES1UG25CS080

#Ashish Rajaniprasad Naik PES1UG25ME009

import wx

import matplotlib.pyplot as plt

app=wx.App()

frame=wx.Frame(None,title="Pie chart",size=(800,500))

frame.Centre()

panel=wx.Panel(frame,style=wx.SIMPLE_BORDER)

frame.Show()

data=wx.TextEntryDialog(panel,"Enter:","User data with comma")

if data.ShowModal()==wx.ID_OK:

   name=data.GetValue()
   
   name=name.split(',')
   
frequency=wx.TextEntryDialog(panel,"Enter:","Data frequency with comma")

if frequency.ShowModal()==wx.ID_OK:

   name1=frequency.GetValue()
   
   name1=name1.split(',')
   
   name1=[float(s) for s in name1]
   
title=wx.TextEntryDialog(panel,"Enter:","Pie chart title")

if title.ShowModal()==wx.ID_OK:

   name2=title.GetValue()
   
plt.figure(figsize=(12, 6))

plt.pie(name1, labels=name, autopct='%1.1f%%', startangle=90)

plt.title(name2)

plt.axis('equal')  

plt.show()

app.Mainloop()

<img width="983" height="743" alt="Screenshot 2025-12-11 221214" src="https://github.com/user-attachments/assets/95534b9c-be46-4894-b80b-a88e759153fa" />
<img width="1136" height="1080" alt="Screenshot 2025-12-11 221324" src="https://github.com/user-attachments/assets/eaef1a7f-a2c7-49e3-a71d-b3ffe315c91f" />
<img width="1149" height="1064" alt="Screenshot 2025-12-11 221358" src="https://github.com/user-attachments/assets/0521b8d8-4531-4408-9b98-3de08e423ae4" />
<img width="1024" height="1068" alt="Screenshot 2025-12-11 221534" src="https://github.com/user-attachments/assets/85ddeb70-6bc4-411d-82b9-3e3a1a4ce377" />


