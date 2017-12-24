# ARP-Poisoning-Detector
Python package to detect ARP poisoning. Supports both python3 and python2. Supports both Windows and Linux.

## Exmaple
```python
from Detector import Detector

poison_results = Detector.Detect()
if poison_results == []:
	print("No poisoning found!")
else:
	print("Poisoning found!")
	for poison_result in poison_results:
		print("	" + ", ".join(poison_result.ip_addresses) + " share the same MAC address.")
```
