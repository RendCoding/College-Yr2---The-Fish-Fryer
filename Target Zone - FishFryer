using UnityEngine;

public class TargetZone : MonoBehaviour
{
    public Collider2D backgroundBar;

    private Collider2D myCollider;

    void Awake()
    {
        myCollider = GetComponent<Collider2D>();
    }

    void Start()
    {
        Randomize();
    }

    public void Randomize()
    {
        float halfWidth = myCollider.bounds.extents.x;
        float minX = backgroundBar.bounds.min.x + halfWidth;
        float maxX = backgroundBar.bounds.max.x - halfWidth;

        float x = Random.Range(minX, maxX);

        transform.position = new Vector3(x, transform.position.y, transform.position.z);
    }
}
