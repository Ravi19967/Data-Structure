#include<stdio.h>
#include<stdlib.h>
struct node
{
	int value;
	struct node *next;
};
struct node *head = NULL;
void push(int item)
{
	struct node *p = (struct node*)malloc(sizeof(struct node));
	if(p == NULL)
	{
		printf("Memory allocation failed");
		return;		
	}
	else
	{
		p->value = item;
		p->next = head;
		head = p;
	}
}
int pop()
{
	if(head != NULL)
	{	
		struct node *temp = head;
		head = head->next;
		return temp->value;
	}	
	else
	{	
		printf("Underflow");
		return -1;
	}
}
int main()
{
	push(10);
	push(29);	
	int value =pop();
	printf("%d",value);
	value =pop();
	printf("%d",value);
	value =pop();
	printf("%d",value);
}

