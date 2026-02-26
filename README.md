from PyPDF2 import PdfMerger

merger = PdfMerger()

print("PDF Merger developed by Monty")
count = int(input("Enter number of PDF files: "))

for i in range(count):
    pdf = input("Enter PDF file path: ")
    merger.append(pdf)

merger.write("merged.pdf")
merger.close()

print("PDF files merged successfully")
