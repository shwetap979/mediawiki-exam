Namespace Creation:
    Run below commands :
        kubectl apply -f namespace-a.yml
        kubectl apply -f namespace-b.yml
        kubectl apply -f namespace-c.yml
        
    To get the list of namespace :
        kubectl get namespaces  
        
Quota Creation:
    kubectl apply -f compute-quota-1.yaml
    
    To get the list of namespace :
        kubectl describe quota --namespace org-a
        kubectl describe quota --namespace org-b
        kubectl describe quota --namespace org-c
        
        
    kubectl describe quota --all-namespaces      
    
Name:       pods-a
Namespace:  org-a
Resource    Used  Hard
--------    ----  ----
memory      0     200Mi



Name:       pods-b
Namespace:  org-b
Resource    Used  Hard
--------    ----  ----
memory      0     400Mi


Name:       pods-c
Namespace:  org-c
Resource    Used  Hard
--------    ----  ----
memory      0     500Mi
