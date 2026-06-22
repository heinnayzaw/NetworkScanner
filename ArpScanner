import socket

def port_scan(host, ports):
	print(f"Scanning {host}...")
	for port in ports:
		s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
		s.settimeout(0.5)
		result = s.connect_ex((host, port))
		if result == 0:
			print(f" Port {port}: OPEN")
		s.close()

port_scan("127.0.0.1", range(20, 1025))

---------------------------------------------------

import socket

target = input("Enter your target: ")

s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)

s.settimeout(0.5)

for port in range(1, 101):
	result = s.connect_ex((target, port))
	
	if result == 0:
		print(f"[OPEN] port {port}")
	else:
		print(f"[CLOSE] port {port}")
		
	s.close()
