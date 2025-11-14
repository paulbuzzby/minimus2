# Wheel Encoders

I asked CoPilot to summarize the common encoders from the scraped data:

The AS5040 is the largest of these and is available in a SSOP16 and takes about twice the area of the others. OTOH, it is hand-solderable should the need arise.

We need about 6000 RPM which should be within the capabilities of the AS5040. Any of the encoders will have sufficient resolution.

---------------------------------------8<------------------------------------------
**The AS5040 is a 10-bit contactless magnetic rotary encoder with absolute and incremental outputs, ideal for basic angular position sensing.** It complements your existing list by offering a simpler, lower-resolution option compared to the 12–14-bit encoders.

---

### 🧭 Updated Magnetic Encoder Comparison Table

| Model           | Resolution     | Max Speed        | Interface(s)           | Key Features                                                                 | Ideal Use Case                        |
|----------------|----------------|------------------|-------------------------|------------------------------------------------------------------------------|----------------------------------------|
| **AS5040**      | 10-bit         | Moderate          | SSI, PWM, Incremental   | Absolute + incremental output, programmable zero position, contactless       | Basic rotary sensing, encoder replacement |
| **AS5050**      | 10-bit         | Moderate          | SPI (3/4-wire)          | Low power, compact, interrupt output                                        | Entry-level angle sensing |
| **AS5050A**     | 10-bit         | Moderate          | SPI (3/4-wire)          | Stray field immunity, interrupt pin, low standby current                     | Low-power embedded systems |
| **AS5055**      | 12-bit         | Moderate          | SPI (3/4-wire)          | Higher resolution, smart power management, alarm bits                        | Portable devices, servo control |
| **AS5047P-ATSM**| 14-bit         | Up to 28,000 rpm  | SPI, ABI                | DAEC™, low latency, high-speed, robust against stray fields                 | Motor control, optical encoder replacement |
| **AS5147P-HTSM**| 14-bit         | Up to 28,000 rpm  | SPI, PWM, ABI           | DAEC™, AEC-Q100 qualified, -40°C to 150°C range                              | Automotive, industrial motor feedback |
| **MA730**       | 14-bit         | Up to 60,000 rpm  | SPI, ABZ, PWM           | End-of-shaft or off-axis, programmable thresholds, fast acquisition         | Robotics, automotive, high-speed apps |

---

### 🔍 Highlights

- **AS5040** adds incremental output and PWM alongside absolute position, making it versatile for legacy encoder replacement.
- **AS5050A** and **AS5055** are optimized for low power and compact designs.
- **AS5047P** and **AS5147P** offer high-speed, high-resolution feedback with dynamic error compensation.
- **MA730** stands out for its extreme speed capability and flexible mounting options.

Let me know if you'd like help selecting the best encoder for a specific motor or application!
**Here’s a summary of the maximum speed and package options for each encoder in your list.** Most high-end models support speeds up to 28,000 or 60,000 rpm, while simpler ones are designed for moderate-speed applications. Package types vary from compact QFN to standard TSSOP and SSOP formats.

---

### 🧭 Magnetic Encoder Speed & Package Comparison

| Encoder Model     | Max Speed         | Package Options                     |
|------------------|-------------------|-------------------------------------|
| **AS5040**        | Up to 10,000 rpm | SSOP-16 (5.3 × 6.2 mm)     |
| **AS5050**        | Not specified (moderate) | QFN-16 (4 × 4 × 0.85 mm)     |
| **AS5050A**       | Not specified (moderate) | QFN-16 (4 × 4 × 0.85 mm)    |
| **AS5055**        | Not specified (moderate) | QFN-16 (4 × 4 mm), TSSOP-14  |
| **AS5047P-ATSM**  | Up to 28,000 rpm | TSSOP-14 (4.4 mm width)     |
| **AS5147P-HTSM**  | Up to 28,000 rpm | TSSOP-14 (4.4 mm width)     |
| **MA730**         | Up to 60,000 rpm | QFN (exact dimensions not specified) |

---

### 🔍 Notes

- **AS5040** is the only one with a clearly stated speed limit of 10,000 rpm, suitable for moderate-speed applications.
- **AS5047P** and **AS5147P** are optimized for high-speed motor control with robust DAEC™ compensation.
- **MA730** leads in speed, handling up to 60,000 rpm, ideal for robotics and high-speed motors.
- **QFN and TSSOP** packages dominate this category, offering compact footprints for embedded systems.


---------------------------------------8<------------------------------------------

## Magnet Suppliers


These are some suppliers I found:

- MagnetStore:
https://magnetstore.co.uk/disc-magnets/6mm-x-3mm-disc-diametrically-magnetised-neodymium-n52-0-31kg-pull/
about £1 each. The seem pretty big for the job

- AMF Magnets
https://amfmagnets.co.uk/products/neodymium-disc-6mm-x-2mm-diametric-n35
about £0.60 each
Still a large diameter but thinner at least. These are about he size recommended in the AS5040 datasheet

- AMF Magnets
https://amfmagnets.co.uk/products/neodymium-disc-magnet-4mm-x-3mm-n52-diametrically-magnetised
about  £0.60 each
Seems like a much better diameter but quite thick

- magnetexpert
https://www.magnetexpert.com/product/6mm-od-x-3mm-id-x-1mm-thick-diametrically-magnetised-n42-neodymium-magnet-19263
about £0.39 each
These look interesting because of the hole though they are quite thick, they will weigh less than the 6x3 ones above

- magnetexpert
https://www.magnetexpert.com/product/6mm-dia-x-1mm-thick-diametrically-magnetised-n42-neodymium-magnet-20413
about £0.30 each
nice and thin while still being the diameter recommended

- first4magnets
https://www.first4magnets.com/product/6mm-dia-x-1mm-thick-diametrically-magnetised-n42-neodymium-magnet-20413
This is the same company as magnetexpert - same phone number for example.

- Digikey have a range of sizes including
https://www.digikey.co.uk/en/products/detail/radial-magnets-inc/9098/22935757
(3mm dia x 2.5mm)
https://www.digikey.co.uk/en/products/detail/radial-magnets-inc/9083/22935780
(4mm dia x 2.5mm)
and several at 6mm dia x 2.5mm
prices are £0.30 to £0.50 each



The Japanese are, as ever, spoilt for choice with many sizes of diametric magnets:
https://www.neomag.jp/shop/magnets/category_list1.php?cat2_id=1&shape_id=1&magdir_id=2

