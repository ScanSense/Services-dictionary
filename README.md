# Services-dictionary

#!/usr/bin/env python
import pandas as pd
import numpy as np
from ipaddress import IPv4Address
from scapy.all import *
from scapy.layers.inet import IP, ICMP
import socket
from sklearn.ensemble import RandomForestClassifier
import tkinter as tk
from tkinter import messagebox
from tkinter import ttk
from PIL import Image, ImageTk
from tkinter import LEFT
from tkinter import RIGHT
from tkinter import Text
from tkinter import PhotoImage
from tkinter import Label, Message




# Define the mapping of ports to services
services = {
    20: 'FTP Data',
    21: 'FTP Control',
    22: 'SSH',
    23: 'Telnet',
    25: 'SMTP',
    53: 'DNS',
    67: 'DHCP Server',
    68: 'DHCP Client',
    69: 'TFTP',
    80: 'HTTP',
    110: 'POP3',
    119: 'NNTP',
    123: 'NTP',
    135: 'RPC Endpoint Mapper',
    137: 'NetBIOS Name Service',
    138: 'NetBIOS Datagram Service',
    139: 'NetBIOS Session Service',
    143: 'IMAP',
    161: 'SNMP',
    162: 'SNMP Trap',
    389: 'LDAP',
    443: 'HTTPS',
    445: 'Microsoft DS',
    465: 'SMTPS',
    587: 'SMTP (submission)',
    636: 'LDAPS',
    993: 'IMAPS',
    995: 'POP3S',
    1433: 'Microsoft SQL Server',
    1434: 'Microsoft SQL Monitor',
    3306: 'MySQL',
    3389: 'Remote Desktop Protocol',
    5432: 'PostgreSQL',
    5900: 'Virtual Network Computing (VNC)',
    8080: 'HTTP alternate'
}
