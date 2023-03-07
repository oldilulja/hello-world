# hello-world

def calculate_reorder_level(current_stock, min_stock):
  reorder_level = min_stock - current_stock
  return reorder_level

# Main program
current_stock = int(input("Enter the current stock level: "))
min_stock = int(input("Enter the minimum stock level: "))

reorder_level = calculate_reorder_level(current_stock, min_stock)

if reorder_level > 0:
  print("Reorder {} units.".format(reorder_level))
else:
  print("No reorder is necessary.")
