# quiz game
a code of questions and multiple answers
def quizgame():
 questions = [
 {"question":"what is the capital of india?",
  "options":["a. tokoyo","b=nizam","c.india","d.bhutan"],
  "answer":"c"
  },
  {"question":"what is the colour of ozone layer?",
  "options":["a.none","b.black","c.blue","d.orange"],
  "answer":"a"
  },
  {"question":"mention 3 emotions that student should not have",
  "options":["a.love","b=discipline","c.attraction","d.crush"],
  "answer":"a,c,d"}]
 score = 0
 print("welcome to the quiz game!")
 for q in questions:
   print(q["question"])
   for option in q["options"]:
    print(option)
   useranswer = input("enter your answer(a/b/c/d):").lower()
   if useranswer==q["answer"]:
    print("correct!")
    score+=1
   else:
    print(f"quiz over!ur {score}/{len(questions)}")
quizgame()
