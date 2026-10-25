
# Personal Expense Category Predictor

def predict_category(expense):
    expense = expense.lower()

    if expense in ["food", "restaurant", "groceries"]:
        return "Food"
    elif expense in ["bus", "petrol", "train"]:
        return "Transport"
    elif expense in ["shirt", "shoes", "dress"]:
        return "Shopping"
    elif expense in ["book", "pen", "notebook"]:
        return "Education"
    else:
        return "Other"


print("Personal Expense Category Predictor")
print("------------------------------------")

expense = input("Enter your expense: ")
category = predict_category(expense)

print("Predicted Category:", category)
