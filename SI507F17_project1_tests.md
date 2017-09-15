## Write in plain english, what will you do to test everything mentioned in the description

* The class Deck's constructor does not accept input, and you can assume this will always be handled correctly by a programmer using this code.
    - Does Deck(1) raise an exception

    - if self.cards is a list
    - if self.cards has instances/objects of Card class
        - self.cards[0] should be an object of class Card
            - self.assertIsInstance(self.cards[0], Card)
            - self.assertIsInstance(object, Class)
        - test all elements of list for class Card (use for loop)
            - for card_object in self.cards:
                self.assertIsInstance(card_object, Card)

    - length of self.cards
    - Does it print 52 lines
        - str(deck)
            'Ace of Diamonds
            2 of Diamonds
            ...'
        - d_string = str(deck)
          d_list = d_string.split('\n')
          len(d_list) == 52

    - 52 cards are popped
        - deck.pop_card()
        - self.assertRaises(IndexError, deck.pop_card)
