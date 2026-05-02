# Stage 1 - Notification Priority Logic

## Approach

Notifications are prioritized using:

- Placement > Result > Event
- Recent notifications first

## Method

1. Assign weights:
   Placement = 3
   Result = 2
   Event = 1

2. Sort:
   - First by weight (descending)
   - Then by timestamp (latest first)

3. Return top N notifications

## Complexity

O(n log n) due to sorting