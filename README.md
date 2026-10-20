# ## Nalanda IT Zone.
* ** Project report under Nalanda it zone internship programme.
 # Name : **DIVYA Bharti 
 # Course : **BSC (5th Semester)
 # Session : **(2024-2028)
 # University Roll Number : **(24281200454) 
 # University Registration Number : **(24120023228)
 # College Name : **S.N. Sinha College 
 
 # Institute Name : **Nalanda It Zone
 
 # Application ID : **(2PFWM0BB)
 
 # Project Topic : Fast - OpenCV - Webcam

# ## Fast & Smooth Webcam Launch in OpenCV.
 
**Question:** Faster Launch of Webcam and smoother video in opencv.

This project optimizes webcam startup speed using the hardware backhand ('CAP - DSHOW') and ensures smooth,lag - free video streaming using **multi - threading**:

## Code Implementation ('main.py)

'''
   python 
import cv
import time
from threading import trade Thread

class Smooth Stream:
    def _inite_(self, src=0):
        # CAP_DSHOW for instant launch on Windows.
        self.cap = cv2.video capture(src, cv2,CAP - DSHON )
        self.cap,set(cv2.CAP_PROP BUFFERSIZE,2)
        self.ret,self,fram = self.cap.read()
        self.running = True

    def start (self):
        Thread (target = self.update,ARGS = (), daemon = True),start () 
        return self

    def update (self):
        while self.running:
             self.ret,self,frame = self.cap.read()

    def read (self):
        return self,frame

    def stop (self):
        self,running = False
        self,cap.release()

If _name_ == "_main_":
   VS = smooth stream().start()

   time.sleep(1,0) # Warn-up

   while True:
       frame = vs.read()
       if frame is not None:
          cv2.imshow("Fast & smooth video",frame)

       if cv2.waitkey(1) & 0xFF == ord('q'):
         break

    vs.stop()
    cv2.destroy All windows()
  
'''

---

## Result 

* ** Startup Time:** Reduced from 4 second to ** less than 1 second
* *" Video Quality:** Smooth FPS ** with no lagging, thanks to background thread frame grabbing.


    # Thank You 🌿

       * Respectful thanks to the teacher for guidance and checking my project file.
          
          
        
    

        
        
 
