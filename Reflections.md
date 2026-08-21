6. flex: 1 1 280px 
flex-grow: 1 The item can grow beyond its basis if there's a leftover space in the container and 1 is teh share of the leftover space to its siblings.
flex-shrink: 1, this item can shrink below its basis is the container is too narrow to fit everyone.
flex-basis: 280px, the item's starting size is calculated before any growug is applied.
actual width = (container: 900px, 3cards, gap: 20px)
Two gaps = 2*20px = 40px
space available for the cards 900px - 40px = 860px
sum of all cards basis = 3*280px = 840px
left over space = 860 - 640 = 20px
total grow factor = 1 + 1 + 1= 3
each getting 20/3 = 6.67px extra/
each card gets 280 + 6.67 = 287px wide.

7. 1. The outer table stretches every card to match the tallest one(align:stretch), like forcing all pictures frames on a shelf to be the same height even if the photos insife are different sizes.
2. Inside each card(now flex-column), the button has margin-top: auto, whic means "eat up all the empty space above me" so whatever the gap the stretching created gets swallowe by the button's margin, showing it down to the floor of the card.

8. Mobile-first adds complexity going up; desktop first removes complexity going down  and siince most people in Malawi uare on phones buiding for the majority first is teh safest order.

9. Floats escape the flow, so parents had to be tricked using the clearfix into seeing them. Flex items never leavae floaw, so the container always knows their size automatically nothinng to trick.