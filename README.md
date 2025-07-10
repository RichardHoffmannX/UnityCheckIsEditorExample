# UnityCheckIsEditorExample
Unity Check IsEditor Example script

```
using UnityEngine;

public class CheckIsEditor : MonoBehaviour
{
    public bool isEditor = false;
    public bool unityEditor = false;

    // Start is called once before the first execution of Update after the MonoBehaviour is created
    void Start()
    {
        if (Application.isEditor)
        {
            isEditor = true;
        }
        else
        {
            isEditor = false;
        }
#if UNITY_EDITOR
        unityEditor = true;
#else
        unityEditor = false;
#endif
    }

    // Update is called once per frame
    void Update()
    {
        
    }
}
```
