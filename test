TICKET_PRICE = 200

tickets_remaining = 10000

service = 20




def calculate_price(num_tickets):
  tax = TICKET_PRICE * num_tickets * .07
  return (TICKET_PRICE * num_tickets) + service + tax
  
while tickets_remaining >= 1: 
  print(""".....\n.....\n.....\nWELCOME!!!!!!!\n.....\n.....\n.....""")
  print("Tickets are available for the Luke Combs concert!!!!!!!") 
  print("Tickets are $200 a piece!")
  print("There will be a 1 time service charge of $20 per order.")
  print("There are {} tickets remaining.".format(tickets_remaining))
  name = input("What is your name?  ")
  name = name.capitalize()
  num_tickets = input("Hello {}, how many tickets would you like?   ".format(name))
  try:
    num_tickets = int(num_tickets)
    if num_tickets > tickets_remaining:
      raise ValueError("There are only {} tickets left.".format(tickets_remaining))
  except ValueError as err:
      print("Oh no, we ran into an issue. {} Please try again.".format(err))
  else:
    price = calculate_price(num_tickets)
    print("""So for {} tickets at $200/ticket and a 7 percent sales tax.....\n....\nprocessing....\n.....""".format(num_tickets))
    print("Your total due is ${}.".format(price)) 
    confirm = input("Would you like to proceed {}? Y?N  ".format(name))
    if confirm.lower() == "y":
        tickets_remaining -= num_tickets 
        card = int(input("please enter a valid card number  "))       
        while card < 1000000000000001:
          print("The card you entered is not valid and must be 16 digits!")
          card = int(input("please enter a valid card number  "))
        print("Thank you very much!")
        cname = input("Is your name the on the card? Y?N   ")
        if cname.lower() == "y":
          print("ok")
        else:
          actname = input("Please enter the name on the card. ")
          perm = input("Did {} give you permission to use the card? Y?N   " .format(actname))
          if actname.lower() == "y":
            print("ok")
          else:
            print("we dont really care as long as we get paid")
        cvv = int(input("please enter a valid '3' digit code "))
        while cvv < 100:
          print("The number you entered is not valid")
          cvv = int(input("please enter a valid '3' digit code "))
        print("your payment is being processed")
        print(""".....\n.....\n.....\n.....\n.....\n.....\n.....\nyour payment is being processed\n.....\n.....\n.....\n.....\n.....""")
        print("payment confirmed")
        ask = input("Is there anything else you would like? ")
        if ask.lower() == "y":
          print("ok")
          print("Please call Big Willie at 828-DEEZ-NUTS!")
        else:
              print("ok")
    else:
      print("Thank you anyways.")
print("Sorry tickets are sold out. :(")
