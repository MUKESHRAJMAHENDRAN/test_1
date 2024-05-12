Contains Duplicate
Solved
Easy
Topics
Companies
Given an integer array nums, return true if any value appears at least twice in the array, and return false if every element is distinct.

 

Example 1:

Input: nums = [1,2,3,1]
Output: true
Example 2:

Input: nums = [1,2,3,4]
Output: false
Example 3:

Input: nums = [1,1,1,3,3,4,3,2,4,2]
Output: true


```
def containsDuplicate(nums):
    # Create an empty set to store unique elements
    seen = set()

    # Iterate through the array
    for num in nums:
        # If the current element is already in the set, return True
        if num in seen:
            return True
        # Otherwise, add the current element to the set
        seen.add(num)

    # If the loop completes without finding any duplicates, return False
    return False

# Test cases
print(containsDuplicate([1,2,3,1]))  # Output: True
print(containsDuplicate([1,2,3,4]))  # Output: False
print(containsDuplicate([1,1,1,3,3,4,3,2,4,2]))  # Output: True

```

    True
    False
    True



```
!pip install nbconvert
```

    Defaulting to user installation because normal site-packages is not writeable
    Requirement already satisfied: nbconvert in /home/mukesh/.local/lib/python3.10/site-packages (7.2.10)
    Requirement already satisfied: beautifulsoup4 in /home/mukesh/.local/lib/python3.10/site-packages (from nbconvert) (4.11.2)
    Requirement already satisfied: bleach in /home/mukesh/.local/lib/python3.10/site-packages (from nbconvert) (6.0.0)
    Requirement already satisfied: defusedxml in /home/mukesh/.local/lib/python3.10/site-packages (from nbconvert) (0.7.1)
    Requirement already satisfied: jinja2>=3.0 in /home/mukesh/.local/lib/python3.10/site-packages (from nbconvert) (3.1.2)
    Requirement already satisfied: jupyter-core>=4.7 in /home/mukesh/.local/lib/python3.10/site-packages (from nbconvert) (5.3.0)
    Requirement already satisfied: jupyterlab-pygments in /home/mukesh/.local/lib/python3.10/site-packages (from nbconvert) (0.2.2)
    Requirement already satisfied: markupsafe>=2.0 in /usr/lib/python3/dist-packages (from nbconvert) (2.0.1)
    Requirement already satisfied: mistune<3,>=2.0.3 in /home/mukesh/.local/lib/python3.10/site-packages (from nbconvert) (2.0.5)
    Requirement already satisfied: nbclient>=0.5.0 in /home/mukesh/.local/lib/python3.10/site-packages (from nbconvert) (0.7.2)
    Requirement already satisfied: nbformat>=5.1 in /home/mukesh/.local/lib/python3.10/site-packages (from nbconvert) (5.7.3)
    Requirement already satisfied: packaging in /home/mukesh/.local/lib/python3.10/site-packages (from nbconvert) (23.0)
    Requirement already satisfied: pandocfilters>=1.4.1 in /home/mukesh/.local/lib/python3.10/site-packages (from nbconvert) (1.5.0)
    Requirement already satisfied: pygments>=2.4.1 in /home/mukesh/.local/lib/python3.10/site-packages (from nbconvert) (2.14.0)
    Requirement already satisfied: tinycss2 in /home/mukesh/.local/lib/python3.10/site-packages (from nbconvert) (1.2.1)
    Requirement already satisfied: traitlets>=5.0 in /home/mukesh/.local/lib/python3.10/site-packages (from nbconvert) (5.9.0)
    Requirement already satisfied: platformdirs>=2.5 in /home/mukesh/.local/lib/python3.10/site-packages (from jupyter-core>=4.7->nbconvert) (3.1.1)
    Requirement already satisfied: jupyter-client>=6.1.12 in /home/mukesh/.local/lib/python3.10/site-packages (from nbclient>=0.5.0->nbconvert) (8.0.3)
    Requirement already satisfied: fastjsonschema in /home/mukesh/.local/lib/python3.10/site-packages (from nbformat>=5.1->nbconvert) (2.16.3)
    Requirement already satisfied: jsonschema>=2.6 in /home/mukesh/.local/lib/python3.10/site-packages (from nbformat>=5.1->nbconvert) (4.17.3)
    Requirement already satisfied: soupsieve>1.2 in /home/mukesh/.local/lib/python3.10/site-packages (from beautifulsoup4->nbconvert) (2.4)
    Requirement already satisfied: six>=1.9.0 in /usr/lib/python3/dist-packages (from bleach->nbconvert) (1.16.0)
    Requirement already satisfied: webencodings in /home/mukesh/.local/lib/python3.10/site-packages (from bleach->nbconvert) (0.5.1)
    Requirement already satisfied: attrs>=17.4.0 in /home/mukesh/.local/lib/python3.10/site-packages (from jsonschema>=2.6->nbformat>=5.1->nbconvert) (22.2.0)
    Requirement already satisfied: pyrsistent!=0.17.0,!=0.17.1,!=0.17.2,>=0.14.0 in /home/mukesh/.local/lib/python3.10/site-packages (from jsonschema>=2.6->nbformat>=5.1->nbconvert) (0.19.3)
    Requirement already satisfied: python-dateutil>=2.8.2 in /home/mukesh/.local/lib/python3.10/site-packages (from jupyter-client>=6.1.12->nbclient>=0.5.0->nbconvert) (2.8.2)
    Requirement already satisfied: pyzmq>=23.0 in /home/mukesh/.local/lib/python3.10/site-packages (from jupyter-client>=6.1.12->nbclient>=0.5.0->nbconvert) (25.0.2)
    Requirement already satisfied: tornado>=6.2 in /home/mukesh/.local/lib/python3.10/site-packages (from jupyter-client>=6.1.12->nbclient>=0.5.0->nbconvert) (6.2)
    
    [1m[[0m[34;49mnotice[0m[1;39;49m][0m[39;49m A new release of pip is available: [0m[31;49m23.2.1[0m[39;49m -> [0m[32;49m23.3.2[0m
    [1m[[0m[34;49mnotice[0m[1;39;49m][0m[39;49m To update, run: [0m[32;49mpython3 -m pip install --upgrade pip[0m



```

```
