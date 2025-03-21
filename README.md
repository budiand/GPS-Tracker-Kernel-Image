## GPS Tracker  

Within this project, I implemented a minimalistic Linux distribution using:  
- **Linux configurations**  
- **Linux system services**  
- **Python scripts**
- **Linux serial interface (UART/TTY)**
- **Space optimization**  

The entire source code, as well as the kernel image, can be found at the following link:  
[GPS Tracker Source Code & Kernel Image](https://drive.google.com/drive/folders/1a1rVeMVb3jAJu5Gn4dEu2-Mv5nFqtIhF?usp=sharing)

---

## How to Test  

1. **Setup and Run the System**  
   - Decompress the `bin_archive.tar.xz` folder and run the launch script:  
     ```sh
     ./launch.sh
     ```
   - The system runs on **QEMU**, so make sure you have it installed beforehand.  
   - Once QEMU starts, log in using:  
     - **User:** `root`  
     - **Password:** `tema2`  

2. **Access the Server**  
   - Open the server at:  
     ```
     http://ip_addr_host:8888
     ```  

3. **Simulate GPS Data**  
   - In another terminal, run:  
     ```sh
     python3 gps-emu.py
     ```
   - The server should display a **hardcoded location** along with the **real UTC time**.
   - You should be able to see something like this:![image](https://github.com/user-attachments/assets/073e507f-eb69-46b4-9d1a-a81f9a199e4d)

