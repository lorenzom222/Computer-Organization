# Representing & Manipulating Info
#### Intro
1. **Binary Digits (Bits):** Modern computers use binary digits, or bits, which are signals that can have only two values: 0 and 1. These bits are the foundation of digital computing.

2. **Decimal vs. Binary:** While decimal (base-10) numbering has been used for centuries, binary notation is more suitable for computers. Decimal works well for humans, who have ten fingers, but binary is more efficient for machines.

3. **History of Decimal:** Decimal numbering has a long history, dating back over 1,000 years and originating in India. It was further developed by Arab mathematicians in the 12th century and introduced to the West by Leonardo Pisano, also known as Fibonacci, in the 13th century.

4. **Advantages of Binary:** Binary values, being two-valued (0 and 1), are well-suited for representing, storing, and transmitting information. For example, they can represent the presence or absence of a hole in a punched card, high or low voltage in electronic circuits, or the orientation of a magnetic domain.

5. **Simplicity and Reliability:** Electronic circuits designed to work with two-valued signals (binary) are simple and reliable. This simplicity allows manufacturers to integrate millions or even billions of such circuits onto a single silicon chip, making modern computing devices compact and powerful.

#### Application

1. **Single Bits:** A single bit, which can be either 0 or 1, doesn't provide meaningful information by itself. It's the smallest unit of data in computing.

2. **Grouping Bits:** To make sense of binary data, we group bits together into sequences. These sequences can represent various things when interpreted in specific ways.

3. **Interpretation:** To give meaning to these bit patterns, we need to interpret them. For instance, by using a binary number system, we can group bits to represent nonnegative numbers. Each unique combination of bits corresponds to a specific number.

4. **Character Encoding:** By applying a standard character code (like ASCII or Unicode), we can encode letters, symbols, and characters used in documents. Each character is assigned a unique bit pattern.

5. **Various Encodings:** The passage mentions that the chapter covers different encodings, including those for representing negative numbers and approximating real numbers. This shows that bits can be used to represent a wide range of data types.

#### Encoding of Numbers
- **Unsigned**: These representation use traditional binary notion and are used for nums >= 0.
    - All values are considered positive
    - Don't have sign to signify "+" or "-"
    - Standard way to represent whole numbers in binary such as: 0, 1, 2, 3, etc.

- **Two's Complement**: Way to represent signed integers, positive and negative
    - Bit Pattern: Leftmost bit represents sign (0 = Positive, 1 = Negative), Remaining represent number
- **Floating-Point**: Way to represent real numbers, such as decimals.

## Info Storage

