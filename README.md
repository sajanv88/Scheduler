# Scheduler

This is a coding test for a job.

## Installing

If you want to install this:

```
git clone https://github.com/GenericJam/Scheduler.git

cd Scheduler

npm install
```

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the most basic way.

### `npm test`

Launches the test suite.<br>

## Project brief

## Factory Managment

In our factory, you are responsible for planning the usage of assembly line for our Supply Chain. ​ Therefore you've decided to organize things a bit by planning everybody’s tasks. The logic is simple: the higher the number of bikes which can be assembled, the more people you can satisfy.
Rules

Sales People give you the starting day of their production cycle and the number of consecutive days they need to reserve the assembly line.

    For example:

    Production Starting Day Duration
    A 02-01-2018 5
    B 09-01-2018 7
    C 15-01-2018 6
    D 09-01-2018 3

```
    Production A starts on day 2 and ends on day 6

    Production B starts on day 9 and ends on day 15

    Production C starts on day 15 and ends on day 20

    Production D starts on day 9 and ends on day 11
```

In this example, it’s not possible to carry out all the productions because the periods for B and C overlap. 3 productions maximum can be carried out: A, D and C.<br/>

Constraints

startingDay > current date

0 < quantity of possible schedules < 100000

0 < duration < 1000

## Examples

Input

```
[
  { "startingDay": "2018-01-02T00:00:00.000Z", "duration": 5 },
  { "startingDay": "2018-01-09T00:00:00.000Z", "duration": 7 },
  { "startingDay": "2018-01-15T00:00:00.000Z", "duration": 6 },
  { "startingDay": "2018-01-09T00:00:00.000Z", "duration": 3 }
]
```

Output

```
{ "productionCycle" : 3 }
```

Input

```
[
  {
  "startingDay": "2018-01-03T00:00:00.000Z",
  "duration": 5
  },
  {
  "startingDay": "2018-01-09T00:00:00.000Z",
  "duration": 2
  },
  {
  "startingDay": "2018-01-24T00:00:00.000Z",
  "duration": 5
  },
  {
  "startingDay": "2018-01-16T00:00:00.000Z",
  "duration": 9
  },
  {
  "startingDay": "2018-01-11T00:00:00.000Z",
  "duration": 6
  }
]
```

Output

```
{ "productionCycle" : 4 }
```
