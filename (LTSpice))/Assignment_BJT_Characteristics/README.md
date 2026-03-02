# BJT Characterization – 2N2222

## Part B – Analysis

### 1) Is IC ≈ βIB perfectly linear?

No. The relationship is approximately linear in the active region, but not perfectly linear.  
The collector current increases roughly proportionally with base current, but β is not constant and varies slightly with operating point.  
Additionally, due to the Early effect, IC increases slightly with VCE.

---

### 2) Estimated β at Three Operating Points

Using:

β = IC / IB

- IB = 0.1 mA → IC ≈ 15 mA → β ≈ 150  
- IB = 0.5 mA → IC ≈ 75 mA → β ≈ 150  
- IB = 1.0 mA → IC ≈ 150 mA → β ≈ 150  

β remains approximately constant in the active region.

---

### 3) Role of V1 = 10 V

The 10 V supply ensures that VCE is large enough to keep the transistor in the active region.

If VCE were very small, the transistor would enter saturation, and IC would no longer follow βIB.
