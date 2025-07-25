# 🏦 ATM Banking System (x86 Assembly – EMU8086)

This is a **console-based ATM Banking System** developed in **x86 Assembly Language**, specifically designed to run on the **EMU8086 emulator**. The application simulates essential banking operations such as login, balance inquiry, money withdrawal, and money transfer — all implemented using DOS interrupts and low-level logic.

---

## 🎯 Features

### 🔐 Secure Login
- Prompts the user to enter a password before accessing the system.
- Character-by-character password validation with masking.

### 💰 Main Menu Options
1. **Balance Inquiry**  
   - Displays total and available balance.
2. **Money Withdrawal**  
   - Offers fixed withdrawal amounts (from $500 to $20,000).
   - Simulates deduction and updates displayed balance.
3. **Money Transfer**  
   - Requires re-entering the password and account number.
   - Follows the same options as withdrawal.
4. **Exit**  
   - Gracefully exits the system with a thank-you message.

### 🧾 Transaction Details
- Predefined balance updates after transactions.
- Simulated outputs for different balance tiers.

### 🧰 Utility Features
- **Error Handling**: Displays invalid input message for incorrect entries.
- **Back Option**: Lets the user return to the main menu.
- **Screen Clearing**: Refreshes the console using `INT 10h` for a cleaner interface.

---

## 🧠 Key Concepts Applied

- **Assembly Programming**: Loops, conditions, branching, and user input/output via `INT 21h`.
- **Screen Handling**: Uses BIOS interrupts to clear and manage display.
- **Procedural Flow**: Organized structure using `call` and labeled code blocks.
- **Password Matching**: Secure character-by-character validation.
- **Menu-Driven Navigation**: User interacts via keyboard selections.

---

## 💻 Technology Stack

- **Language**: x86 Assembly (Real Mode, 16-bit)
- **IDE / Emulator**: [**EMU8086**](http://www.emu8086.com/)
- **Instructions Used**: `INT 21h`, `INT 10h`, loops, conditionals
- **Platform**: Windows (via EMU8086)

---

## 🏁 How to Run (EMU8086)

1. Open EMU8086.
2. Load the `.asm` file (e.g., `atm.asm`).
3. Compile and run using **F5** or the "Compile + Run" option.
4. Interact using keyboard input as prompted.

---

## 📌 Notes

- The login password is hardcoded as: `pasword`
- All transactions are simulated; balance updates are not calculated dynamically.
- Ideal for demonstrating low-level banking logic and DOS-based console interaction using Assembly.

---
