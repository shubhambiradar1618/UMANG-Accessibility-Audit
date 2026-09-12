# UMANG Accessibility Audit

## 1. Website Information

- **Website:** UMANG
- **URL:** https://web.umang.gov.in/
- **Audit Tool:** Microsoft Edge Lighthouse
- **Device:** Desktop
- **Accessibility Score:** 90/100

## 2. Audit Objective

The objective of this audit is to identify accessibility
and keyboard-navigation issues on the UMANG public-facing
website and recommend suitable improvements.

## 3. Accessibility Findings

### Issue 1 – Missing Accessible Names

**Severity:** High

**Finding:**  
Some button, link, and menuitem elements do not have
accessible names.

**Impact:**  
Screen-reader users may not understand the purpose of
affected interactive controls.

**Recommended Fix:**  
Add meaningful accessible names using visible text,
appropriate labels, or suitable ARIA attributes.

**Evidence:**  
Lighthouse Accessibility audit screenshot.

---

### Issue 2 – Positive tabindex Values

**Severity:** High

**Finding:**  
Some elements have a tabindex value greater than 0.

**Impact:**  
This can create an unexpected keyboard navigation order.

**Recommended Fix:**  
Avoid positive tabindex values and use the natural DOM
order wherever possible.

**Evidence:**  
Lighthouse audit screenshot.

---

### Issue 3 – Incorrect Heading Order

**Severity:** Medium

**Finding:**  
Heading elements are not in a sequentially-descending order.

**Impact:**  
Screen-reader users may have difficulty understanding
the page structure.

**Recommended Fix:**  
Use a logical heading hierarchy such as H1, H2 and H3.

**Evidence:**  
Lighthouse audit screenshot.

---

### Issue 4 – Missing Main Landmark

**Severity:** Medium

**Finding:**  
The document does not have a main landmark.

**Impact:**  
Assistive-technology users may have difficulty quickly
accessing the primary page content.

**Recommended Fix:**  
Use a semantic `<main>` element around the primary content.

**Evidence:**  
Lighthouse audit screenshot.

---

### Issue 5 – Keyboard Navigation Review

**Severity:** Medium – Pending Manual Verification

**Finding:**  
Keyboard-only navigation requires manual verification to
ensure that all interactive elements are reachable and that
the focus order is logical.

**Impact:**  
Keyboard-only users may face difficulty if focus is skipped,
moves unexpectedly, or is not clearly visible.

**Recommended Fix:**  
Test the website using Tab, Shift+Tab, Enter and Escape.
Ensure all interactive elements are reachable and that focus
is clearly visible.

**Evidence:**  
Manual keyboard navigation test.

## 4. Remediation Priority

1. Missing accessible names – High
2. Positive tabindex values – High
3. Incorrect heading hierarchy – Medium
4. Missing main landmark – Medium
5. Keyboard navigation review – Medium

## 5. Conclusion

The UMANG website achieved an Accessibility score of 90/100
during the Lighthouse audit. The audit identified several
accessibility improvements related to interactive controls,
keyboard navigation and semantic page structure.

Addressing these issues can improve usability for keyboard
users and users of assistive technologies.
