# CheckLastEventStatus UseCase

## Data
* Group Id

## Primary flow
1. Get the last data group's event (end data and grade market end)
2. Return status "active" if the event not finished yet.

## Alternative flow: The event is on end edge
2. Return status "active"

## Alternative flow: Event is ended, in grade market period though
2. Return status "on review"

## Alternative flow: Event and grade market ended
2. Return "ended"

## Alternative flow: Group hasn't any event checked
2. Return status "ended"